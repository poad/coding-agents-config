# Coding Agents Configuration

このリポジトリは、複数のAIコーディングエージェントの設定ファイルを管理するためのものです。

## 概要

以下のAIコーディングエージェントの設定ファイルが含まれています：

- **Amazon Q Developer** - AWSが提供するAIコーディングアシスタント
- **Claude** - AnthropicのAIアシスタント
- **Codex CLI** - OpenAIのCodexを使用したCLIツール
- **opencode** - オープンソースのAIコーディングツール

## ディレクトリ構成

```text
.
├── amazon-q-developer/    # Amazon Q Developerの設定
│   └── amazonq/
│       ├── mcp.json      # MCP（Model Context Protocol）サーバー設定
│       └── ...
├── claude/               # Claudeの設定
│   └── .claude/
│       ├── .mcp.json     # MCP設定
│       └── ...
├── codex/                # Codex CLIの設定
│   └── .codex/
│       ├── config.toml   # Codex設定ファイル
│       └── ...
└── opencode/             # opencodeの設定
    └── opencode/
        ├── opencode.json # opencode設定ファイル
        └── ...
```

## セットアップ

各エージェントの設定が入っているサブディレクトリのREADME.mdを

## 関連リンク

### Amazon Q Developer リンク

- [Amazon Q Developer](https://developer.amazon.com/ja-jp/amazon-q)
- [GitHub - amazon-q-developer/amazon-q-cli](https://github.com/aws/amazon-q-developer-cli/tree/main)
- [VS Code extension](https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.amazon-q-vscode)

### Claude リンク

- [Claude](https://claude.ai/)

### Codex CLI リンク

- [Codex CLI](https://developers.openai.com/codex/cli)
- [GitHub - openai/codex-cli](https://github.com/openai/codex)

### opencode リンク

- [opencode](https://opencode.ai/)
- [GitHub - sst/opencode](https://github.com/sst/opencode)
- [VS Code extension](https://marketplace.visualstudio.com/items?itemName=sst-dev.opencode)

## 注意事項

- 各エージェントの設定ファイルには、APIキーやトークンなどの機密情報が含まれる場合があります
- 設定ファイルを共有する際は、機密情報を削除してください
- 各エージェントの最新の設定方法については、公式ドキュメントを参照してください
