# Cat Image MCP Server

猫画像を取得するMCPサーバーです。The Cat APIを使用してランダムな猫画像を取得し、base64エンコードしたデータを返します。

## セットアップ

1. 依存関係をインストール:
```bash
npm install
```

2. The Cat APIのAPIキーを取得し、環境変数に設定:
```bash
export CAT_API_KEY="your_api_key_here"
```

## 使用方法

このサーバーはMCPツールとして動作し、以下の機能を提供します:

- `get-cat-image`: ランダムな猫画像を取得

### 例

```javascript
const result = await mcp.useTool(cat-image, get-cat-image);
// result.content[0].data にbase64エンコードされた画像データが含まれます
```

## 依存関係

- [@modelcontextprotocol/sdk](https://github.com/modelcontextprotocol/sdk)
- [zod](https://github.com/colinhacks/zod)
- [The Cat API](https://thecatapi.com/)

## 実行方法

```bash
npm start
```

## ライセンス

ISC
