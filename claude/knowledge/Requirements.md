# SIMS Requirements

Version: 3.0 Draft

## 目的

SIMSは、Google Search Consoleのデータとブログ内Knowledgeを利用し、既存記事を継続的に改善するためのSEO改善システムである。

SIMSは新規記事作成システムではない。

主目的は以下である。

- 検索意図とのズレを修正する
- CTRを改善する
- 検索順位を改善する
- 内部リンクを最適化する
- 古い情報を更新する
- カニバリを防ぐ
- 改善結果をLearningとして蓄積する

---

## 対象ユーザー

SIMSは以下の運営者を対象とする。

- AdSenseブログ運営者
- 既存記事を改善したいブログ運営者
- Search Consoleを利用している運営者
- 複数カテゴリの記事を管理している運営者
- Claude ProjectでSEO改善を行いたい運営者

---

## 入力データ

SIMSが扱う入力は以下である。

### 必須

- 改善対象記事の本文
- Search Consoleデータ
- メインキーワード
- 記事URL

### 推奨

- Knowledge内の記事一覧
- Hub_Map
- Keyword_Map
- 過去のLearning

---

## 出力データ

SIMSは以下を出力する。

- 改善済み完成記事
- titleタグ
- meta description
- 改善タグ
- 内部リンク提案
- 投稿前チェックリスト
- Publishing Summary
- Learning更新案

---

## Knowledgeの役割

Knowledgeは、ブログ全体の構造化データである。

KnowledgeはClaude Projectで参照するMarkdownファイルとして管理する。

Knowledge_MasterはGoogleスプレッドシートで管理する正本であり、Claude ProjectにはMarkdown化したKnowledgeのみを配置する。

---

## Engineの役割

Engine01〜Engine10は、記事改善の工程を分担する。

各Engineは責務を分離し、前のEngineの出力を次のEngineへ渡す。

EngineはKnowledgeを参照してよいが、Knowledgeを直接書き換えない。

---

## 改善方針

SIMSは以下の優先順位で改善する。

1. 読者利益
2. 検索意図
3. E-E-A-T
4. SEO
5. CTR
6. 内部リンク
7. 収益化

順位改善だけを目的にしない。

---

## 禁止事項

SIMSでは以下を禁止する。

- 存在しない記事への内部リンク
- KnowledgeにないURLの推測
- 検索意図を無視したリライト
- 過剰なキーワード詰め込み
- 根拠のない断定
- YMYL領域での無根拠な助言
- Engineの責務をまたいだ処理

---

## 運用フロー

基本フローは以下である。

1. Search Consoleで改善対象記事を選ぶ
2. 対象記事本文とSearch Consoleデータを用意する
3. SIMSでEngine01〜Engine09を実行する
4. 完成記事をブログへ反映する
5. 2〜4週間後にEngine10で効果を分析する
6. Learningへ改善結果を蓄積する

---

## Version方針

Version3.0では以下を固定する。

- Knowledgeはカテゴリ別Markdownで管理する
- Knowledge_Masterは正本としてGoogleスプレッドシートで管理する
- Claude ProjectにはMarkdown Knowledgeのみ配置する
- KB00〜KB99方式は廃止する
- Engine01〜10を正式な処理単位として維持する
