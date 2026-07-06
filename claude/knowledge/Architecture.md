# SIMS Architecture

Version: 3.0 Draft

---

# Overview

SIMS（Search Intent Management System）は

Google Search Console

Knowledge

Claude

を連携し、

既存記事を改善するSEO改善プラットフォームである。

---

# Architecture

```
Search Console
        │
        ▼
 Improvement Request
        │
        ▼
 Project Instructions
        │
        ▼
 Engine01
        │
        ▼
 Engine02
        │
        ▼
 Engine03
        │
        ▼
 Engine04
        │
        ▼
 Engine05
        │
        ▼
 Engine06
        │
        ▼
 Engine07
        │
        ▼
 Engine08
        │
        ▼
 Engine09
        │
        ▼
 Improvement Result
        │
        ▼
 Engine10
        │
        ▼
 Learning
```

---

# Components

SIMSは以下のコンポーネントで構成される。

## Core

Project Instructions

ProjectFiles

README

CHANGELOG

---

## Engine

Engine01〜Engine10

責務を分離して処理する。

---

## Knowledge

Knowledgeはブログ全体の構造化データである。

```
Knowledge

Blog_Profile.md

Articles/

Windows.md

AI.md

Apple.md

Android.md

Microsoft365.md

WordPress.md

SNS.md

Gadget.md

Video.md

Productivity.md

Other.md

Hub_Map.md

Keyword_Map.md

Learning.md
```

---

## Knowledge Master

唯一の正本

Googleスプレッドシート

↓

Knowledge Builder

↓

Knowledge

Knowledge_Masterは

Claude Projectへ置かない。

---

# Engine Responsibility

Engine01

検索意図分析

---

Engine02

競合分析

---

Engine03

EEAT改善

---

Engine04

構成改善

---

Engine05

本文改善

---

Engine06

SEO最適化

---

Engine07

CTR改善

---

Engine08

Knowledge参照

内部リンク

関連記事

Hub

Keyword

Learning参照

---

Engine09

最終チェック

完成記事生成

Publishing Summary

---

Engine10

順位改善分析

Learning更新

---

# Knowledge Flow

```
Knowledge_Master

↓

Knowledge Builder

↓

Knowledge

↓

Engine08

↓

Engine09
```

---

# Search Console Flow

```
Search Console

↓

改善対象選定

↓

Engine01

↓

Engine09

↓

公開

↓

Engine10

↓

Learning
```

---

# Learning Flow

```
改善

↓

順位変化

↓

CTR変化

↓

Learning更新

↓

次回改善へ反映
```

---

# Design Principles

SIMSでは

Engine

Knowledge

Learning

を分離する。

Knowledgeは

Engineから編集しない。

Learningは

Engine10のみ更新する。

---

# Version

SIMS Version3.0 Draft
