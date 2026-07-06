# SIMS Data Model

Version: 3.0 Draft

---

# Purpose

DataModelは

SIMSで利用する全データの構造を定義する。

Knowledge

Learning

Engine

Search Console

は

すべてこのモデルに従う。

---

# Entity

SIMSでは以下を管理する。

・Article

・Hub

・Keyword

・Learning

・Blog

---

# Article

記事を管理する。

必須項目

| Field | Required | Description |
|---------|----------|-------------|
| ArticleID | Yes | 一意ID |
| Title | Yes | 記事タイトル |
| URL | Yes | 公開URL |
| Category | Yes | カテゴリ |
| MainKW | Yes | メインKW |
| SubKW | No | サブKW |
| SearchIntent | Yes | 検索意図 |
| SearchStage | No | 検索段階 |
| ArticleType | Yes | 記事タイプ |
| Summary | Yes | 要約 |
| Priority | No | 優先度 |
| ContentStatus | Yes | 状態 |
| Hub | No | HubID |
| LastUpdated | Yes | 更新日 |

---

# Hub

内部リンク構造

| Field | Description |
|---------|-------------|
| HubID | Hub識別子 |
| HubTitle | Hubタイトル |
| Parent | 親記事 |
| Child | 子記事 |
| Relationship | 関係 |
| Priority | 優先度 |

---

# Keyword

検索意図管理

| Field | Description |
|---------|-------------|
| MainKW | メインKW |
| RelatedKW | 関連KW |
| Intent | Intent |
| ArticleID | 対象記事 |
| Difficulty | 難易度 |
| Volume | 検索数 |

---

# Learning

改善履歴

| Field | Description |
|---------|-------------|
| Date | 日付 |
| ArticleID | 対象記事 |
| BeforeRank | 改善前順位 |
| AfterRank | 改善後順位 |
| BeforeCTR | 改善前CTR |
| AfterCTR | 改善後CTR |
| Action | 実施内容 |
| Result | 結果 |
| Notes | 備考 |

---

# Blog

ブログ全体情報

| Field | Description |
|---------|-------------|
| BlogName | ブログ名 |
| Domain | ドメイン |
| Theme | テーマ |
| Target | 読者 |
| Monetization | 収益化 |
| Categories | カテゴリ一覧 |

---

# Relationships

Blog

↓

Article

↓

Hub

↓

Keyword

↓

Learning

---

# Data Rules

ArticleIDは変更しない。

URL変更後も

ArticleIDは維持する。

Hubは

ArticleIDで管理する。

Learningは

ArticleIDで管理する。

Keywordは

ArticleIDへ紐付ける。

---

# Source of Truth

唯一の正本

Knowledge_Master

Googleスプレッドシート

↓

Knowledge Builder

↓

Markdown

↓

Claude Project

---

# Version

SIMS Version3.0 Draft
