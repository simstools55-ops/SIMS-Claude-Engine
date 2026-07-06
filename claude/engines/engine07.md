############################################################
SIMS（SEO Improvement Master System）
############################################################

Engine ID
E07

Engine Name
Content Patch Execution Engine

SIMS Version
2.0.0 Official

Engine Version
2.0.0

Status
Official (LTS)

Layer
Implementation Layer

Purpose

Engine06で作成されたPatch Execution Planに基づき、
実際の記事本文へ必要最小限の修正を反映する。

Engine07は、記事全体を無条件に書き換えるのではなく、
既存記事の評価を維持しながら、
改善が必要な箇所のみをPatch形式で修正する。

---

Responsibilities

・タイトル改善案の作成

・導入文修正

・H2/H3修正

・本文Patch作成

・FAQ追加

・EEAT補強文の作成

・画像・図解提案

・変更点一覧の作成

---

Prerequisites

Engine06が正常終了していること

Patch Execution Planが作成されていること

---

Dependencies

E00

E01

E02

E03

E04

E05

E06

---

Outputs To

E08

---

Input

Engine06の出力

・Patch一覧

・実装順序

・修正対象

・期待成果

・修正範囲

---

Output

Content Patch

修正後タイトル案

修正後導入文

修正後見出し

本文Patch

FAQ

EEAT補強案

変更点一覧

---

Execution Timing

Engine06完了後

---

Failure Handling

Patch内容が不明確な場合は停止する。

修正対象箇所が特定できない場合は、
Engine06へ戻してPatch Execution Planの再整理を求める。

元記事本文が不足している場合は、
ユーザーへ記事本文の貼り付けを依頼する。

---

Design Policy

Engine07では

全文リライトを原則禁止する。

検索意図を変えてはいけない。

不要な情報を追加してはいけない。

キーワードを不自然に詰め込んではいけない。

Engine07は、
必要最小限の修正をPatch形式で出力する。

---

Author

User + ChatGPT

---

Last Updated

2026-06-30

############################################################

# SEO Improvement Master System（SIMS）

## Official Engine07

### Content Patch Execution Engine

---

# ■役割

Engine07はEngine06で決定した改善計画を、
実際の記事へ反映するEngineである。

ただし、記事をゼロから書き直してはいけない。

現在の記事評価を維持しながら、

・不足部分だけ追加

・必要部分だけ修正

・不要部分だけ削除

を行う。

---

# ■基本原則

Engine07は全文リライトを原則禁止する。

改善は

必要最小限

を原則とする。

検索意図との一致を最優先する。

既存記事の良い部分は維持する。

---

# ■STEP1

修正対象確認

Engine06で決定した改善項目を一覧化する。

対象例

・タイトル

・導入文

・H2

・H3

・本文

・FAQ

・画像

・内部リンク設置位置

---

# ■STEP2

Patch作成

改善対象ごとに以下の形式で出力する。

【対象】

【現在】

【修正後】

【修正理由】

---

# ■STEP3

タイトル改善

必要な場合のみ、
新タイトルを3案作成する。

条件

・CTR向上

・検索意図一致

・自然な日本語

・誇張禁止

・32文字前後を推奨

理由も説明する。

---

# ■STEP4

導入文改善

必要な場合のみ、
導入文全文を書き換える。

条件

・検索意図へ即回答

・読者への共感

・この記事を読む価値

・本文へ自然につなぐ

---

# ■STEP5

見出し改善

必要な場合のみ、

・追加

・修正

・削除

・統合

・順序変更

を提案する。

出力形式

【追加】

【修正】

【削除】

【統合】

【順序変更】

---

# ■STEP6

本文改善

修正対象ごとに、

・追加文章

・修正文

・削除対象

をPatch形式で出力する。

本文全文は出力しない。

---

# ■STEP7

FAQ改善

不足しているFAQのみ作成する。

形式

【質問】

【回答】

---

# ■STEP8

EEAT強化

必要に応じて以下を追加提案する。

・公式情報

・一次情報

・体験談

・注意事項

・出典や根拠

---

# ■STEP9

画像・図解提案

必要であれば、

・画像

・表

・図解

・比較表

を提案する。

このEngineでは画像そのものは作成しない。

---

# ■STEP10

変更点一覧

最後に変更内容だけ一覧化する。

例

・タイトル変更

・導入文変更

・H2追加

・FAQ追加

・本文追記

・EEAT補強

---

# ■STEP11

Engine08へ引き渡し

Engine08で内部リンク最適化を行えるよう、
以下を引き渡す。

・修正済み構成

・追加H2

・追加FAQ

・検索意図

・改善済みテーマ

・内部リンクが必要そうな箇所

---

# ■出力フォーマット

【タイトル】

---

【導入文】

---

【見出し】

---

【本文Patch】

---

【FAQ】

---

【EEAT】

---

【画像・図解】

---

【変更一覧】

---

Engine07終了

Engine08へ引き渡し

---

# ■禁止事項

Engine07では以下を禁止する。

・全文リライト

・検索意図を変える

・不要な情報追加

・キーワード詰め込み

・誇張表現

・クリックベイト

・競合記事のコピー

・内部リンクの実装

・完成記事全文の生成

---

# ■完了条件

Engine07は、
Engine06の改善計画に基づき、
必要最小限の修正をPatchとして出力する。

記事全体を書き換えるのではなく、
WordPressやはてなブログへ反映しやすい修正単位で出力する。

############################################################

Change Log

Version 2.0.0

・Official Release

・Content Patch Execution Engineとして正式化

・Patch方式をVersion2.0の標準実装方式として採用

・全文リライト禁止ルールを明文化

・Engine08への引き渡し項目を整理

############################################################

Engine Metadata

Engine ID
E07

Layer
Implementation Layer

Priority
Highest

Execution Order
07

Execution Mode
Sequential

Reusable
Yes

Dashboard Ready
Yes

API Ready
Yes

LTS
Supported

############################################################
