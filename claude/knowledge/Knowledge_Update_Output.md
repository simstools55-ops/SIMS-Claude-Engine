# Knowledge Update Output

Version: 3.1 Beta

Status: Active

---

# Purpose

記事改善後にKnowledge_Masterへ反映すべき更新候補を出力する。

ClaudeはKnowledge_Master.xlsを直接編集してはならない。

Knowledge_Master_Update_Sheetのみ出力する。

---

# Update Rule

## 上書き

- Summary
- Priority
- UpdateDate

---

## 追記

- Remarks
- Learning Candidate

---

## 更新しない

- ArticleID
- URL
- Category
- MainKW
- SubKW
- SearchIntent
- SearchStage

---

# Output Format

## 更新対象

Sheet：

Knowledge_Master

ArticleID：

XXXX-0000

---

## 上書き

| Column | Rule | New Value |
|---|---|---|
| Summary | 上書き | |
| Priority | 上書き | |
| UpdateDate | 上書き | |

---

## 追記

| Column | Rule | Append Value |
|---|---|---|
| Remarks | 追記 | |
| Learning Candidate | 追記 | |

---

## Google Sheets貼付用TSV

ArticleID	Summary	Priority	UpdateDate	Remarks追記	Learning追記

---

# Rules

Knowledge_Master.xlsは更新しない。

Knowledgeを更新したとは表現しない。

更新候補のみ出力する。

Summary・Priority・UpdateDateは上書きする。

Remarks・Learning Candidateは追記する。

Google Sheetsへ反映するのはユーザーである。
