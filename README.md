# SIMS Claude Engine

SIMS Claude Engine は、SIMS Core から渡される改善依頼書を受け取り、Claude上で記事改善を実行するための独立リポジトリです。

## 役割

- Claude Project Instructions の管理
- SEO改善Engine群の管理
- Knowledge / Templates の管理
- SIMS AI Exchange仕様への対応
- Improvement Request / Result の標準化

## SIMS本体との関係

- SIMS Core: Search Console取得、改善案件管理、履歴管理、効果測定
- SIMS Claude Engine: 記事改善の実行、改善結果の返却

SIMS Coreとは `Improvement_Request.md` と `Improvement_Result.md` を中心に連携します。

## 推奨運用

1. このリポジトリの `claude/instructions/CLAUDE_PROJECT_INSTRUCTIONS.md` をClaude Project Instructionsへ貼り付ける。
2. `claude/engines/` と `claude/knowledge/` をClaude Project Knowledgeへ登録する。
3. SIMS Coreで生成した `Improvement_Request.md` をClaudeへ渡す。
4. Claudeが記事改善と `Improvement_Result.md` を返す。
5. SIMS Coreへ結果を記録する。

## Version

Initial Foundation: v1.0.0
