# SIMS-Claude-Engine v2.0.0 Prototype Baseline

このリポジトリは、運用実績のある `ai-yoshida` プロトタイプをベースラインとして、SIMS AI Exchange v1.0 に接続するための Claude Engine です。

## Claude Projectへ入れるもの

### Project Instructions

`claude/project-instructions/CLAUDE_PROJECT_INSTRUCTIONS_PROTOTYPE_BASELINE.md`

### Project Knowledge

以下をClaude Project Knowledgeへ追加してください。

- `claude/engines/engine00.md` ～ `engine10.md`
- `claude/knowledge/` 配下の主要Knowledge
- `claude/knowledge/category/` 配下のカテゴリKnowledge
- `claude/prompts/RUN_SIMS_AI_EXCHANGE_IMPROVEMENT.md`
- `claude/templates/SIMS_Improvement_Result_v1.0_TEMPLATE.md`

## 方針

- 既存プロトタイプの改善力を維持する
- SIMSから渡される `Improvement_Request` を入力として扱う
- Claudeは `Improvement_Result` 形式で返す
- Engineは安定資産、Knowledgeは運用で更新する

