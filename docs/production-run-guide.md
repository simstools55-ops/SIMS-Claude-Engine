# Claude Engine Production Run Guide

## 目的

SIMSから渡されたImprovement Requestを受け取り、記事改善結果をAI Exchange形式で返す。

## 実行手順

1. SIMSで生成されたImprovement RequestをClaude Projectへ貼り付ける。
2. 必要に応じて記事本文を追加で貼り付ける。
3. Claude Engineに改善を実行させる。
4. Improvement Result形式で出力する。
5. H1、titleタグ、description、スマホ向けdescriptionを必ず含める。
6. Reasoning Summaryを初心者にも分かる言葉で出力する。

## 出力ルール

- Main Queryを明示する。
- Sub Queriesを明示する。
- H1とtitleタグを分けて出力する。
- meta descriptionは通常版とスマホ向けを分ける。
- WordPress反映手順を添える。
- 完了チェックリストを添える。
