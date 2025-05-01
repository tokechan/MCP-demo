# MCP-TODOS

チャット機能付きTODOアプリケーション。AIアシスタントとの対話を通じてTODOの管理ができます。

## プロジェクト構造

```
mcp-todos/
├── api/              # バックエンドAPI（Hono）
├── client/           # フロントエンド（Next.js）
│   ├── app/         # Next.js 13+ App Router
│   │   ├── api/     # APIルート
│   │   ├── globals.css
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   └── QueryProvider.tsx
│   ├── components/  # UIコンポーネント
│   │   └── ui/     # shadcnコンポーネント
│   │       ├── badge.tsx
│   │       ├── button.tsx
│   │       ├── card.tsx
│   │       ├── input.tsx
│   │       └── scroll-area.tsx
│   └── lib/        # ユーティリティ関数
└── mcp/            # MCPサーバー
```

## 技術スタック

- **フロントエンド**
  - Next.js 14.1.0
  - React 18.2.0
  - TypeScript
  - Tailwind CSS
  - shadcn/ui
  - Tanstack Query
  - Framer Motion

- **バックエンド**
  - Hono
  - Model Context Protocol

## セットアップ

### 必要条件
- Node.js v18以上
- npm v9以上

### インストール

1. クライアントの依存関係をインストール:
```bash
cd client
npm install
```

2. 開発サーバーを起動:
```bash
npm run dev
```

アプリケーションは以下のポートで起動します：
- フロントエンド: http://localhost:3000
- バックエンドAPI: http://localhost:8080
- MCPサーバー: http://localhost:3001

## 機能

- チャットベースのTODO管理
- AIアシスタントとの対話
- リアルタイムの更新
- ダークモード対応
- レスポンシブデザイン

## 開発者向け情報

### 使用しているフォント
- Inter（Google Fonts）

### スタイリング
- Tailwind CSSを使用
- shadcn/uiコンポーネントライブラリ
- カスタムカラーテーマ設定

### 状態管理
- Tanstack Query（React Query）を使用したサーバー状態管理

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。 