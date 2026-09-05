# doc-discipline

プロジェクト文書の作成・更新・整理の規律をまとめたエージェント用スキルです。
README、`docs/`、仕様書、コード内のコメントを対象とします。

## 何を扱うか

ソフトウェアを使う人・運用する人・変更する人が、必要な情報を見つけ、正しく使い続けられるように文書を管理します。
契約や検証結果の伝え方、正本と要約・例の関係、文書の寿命、コメントと API 文書、コード変更との同期を扱います。

判断基準の正本は [SKILL.md](SKILL.md) です。
文書の存続は [役割に応じて判断](SKILL.md#文書の役割に合わせて更新保存する) し、
実装と文書の不一致は [合意した契約を基準に解消](SKILL.md#実装と文書が食い違っていたら) します。
レビューの依頼では指摘を報告し、修正が依頼・承認されている場合にその範囲で編集します。

## 使い方

`SKILL.md` は Claude Code、Codex、opencode が共通して読める形式です。
各ツールのスキル探索先へ、このリポジトリを置くか symlink します。

```
~/.claude/skills/doc-discipline/SKILL.md
~/.codex/skills/doc-discipline/SKILL.md
~/.config/opencode/skills/doc-discipline/SKILL.md
```

## 関連するスキル

`design-review` と併用する場合、契約・品質・設計や検証の妥当性はそちらで判断し、
このスキルでは、その契約・理由・根拠を文書が正しく伝え、維持できるかを確認します。
決まった内容をどう書くかは `japanese-technical-writing` が扱います。

- [japanese-technical-writing](https://github.com/libratechw/japanese-technical-writing) — 日本語実用文の書き方。順序、命名、強調、図表の選び方
- [design-review](https://github.com/libratechw/design-review) — 設計と実装のレビュー基準

## 貢献

規則の追加や修正の提案を歓迎します。

提案には、判断を改善できる具体的な事例や、要件・文書に基づく根拠を添えてください。
現在の規則で防げているなら、追加せずに済みます。

## ライセンス

[CC0 1.0](LICENSE) で公開します。
