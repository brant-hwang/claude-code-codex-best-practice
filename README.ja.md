# AIコーディングエージェント セットアップガイド

> **Claude Code + Codex + gstack + Ralph** — AIコーディングエージェントを構造化された仮想開発チームに変える完全ガイド。

**[ガイドを読む](https://ai-coding-guide-with-gstack.vercel.app)**

[한국어](https://ai-coding-guide-with-gstack.vercel.app/ai-coding-setup-guide-ko.html) | [English](https://ai-coding-guide-with-gstack.vercel.app/ai-coding-setup-guide-en.html) | [日本語](https://ai-coding-guide-with-gstack.vercel.app/ai-coding-setup-guide-ja.html)

---

## これは何ですか？

多くの開発者はAIコーディングエージェントを高度なオートコンプリート程度にしか使っていません。このガイドでは、AIエージェントを**役割が分離された開発チーム**として運用する方法を紹介します — 企画、実装、レビュー、QA、デプロイをそれぞれ専門化されたワークフローで処理します。

ゼロから全てをカバーします：

1. **基礎環境** — ターミナル、シェル、Homebrew、Node.js、エディタ設定
2. **Claude Code** — インストール、設定、CLAUDE.mdのベストプラクティス、サブエージェントワークフロー
3. **Codex** — OpenAIのCLIエージェントをセカンドオピニオン＆コードレビュアーとして活用
4. **MCPサーバー** — ブラウザ、GitHub、Slackなどとエージェントを接続
5. **gstack** — 開発プロセスを強制するスキルベースのワークフローエンジン
6. **CLAUDE.md / AGENTS.md** — プロダクションレベルのプロンプト設定
7. **Ralph（Ouroboros）** — スペック優先の自律開発ループ
8. **付録** — Claude Code内部構造、`.claude/`ディレクトリ、フック、パーミッション

## 誰のためのガイドですか？

- AI開発に**構造とプロセス**が必要な**創業者 / テックリード**
- Claude Code、Codex、gstackを初めて使う**開発者**
- 「AIとチャット」を超えて「AIをチームとして運用」したい**すべての方**

## ナビゲーション

スライド形式のプレゼンテーションです：

- **矢印キー**（上下左右すべて）、**Space**、**PageUp/Down**
- **マウスホイール**（縦スクロールが横スライド移動にマッピング）
- モバイルでは**タッチスワイプ**

---

**制作: [Brant Hwang](mailto:brant@querypie.com)** — [QueryPie](https://www.querypie.com) CEO
