[![Next.js](https://img.shields.io/badge/-Next.js-000000.svg?logo=next.js&style=flat)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-%2320232a.svg?logo=react&style=flat)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-%2338B2AC.svg?logo=tailwind-css&style=flat)](https://tailwindcss.com/)
[![oxlint](https://img.shields.io/badge/-oxlint-000000.svg?logo=oxlint&style=flat)](https://oxc.rs/docs/guide/usage/linter)
[![oxfmt](https://img.shields.io/badge/-oxfmt-000000.svg?logo=oxfmt&style=flat)](https://oxc.rs/docs/guide/usage/formatter.html)
[![lefthook](https://img.shields.io/badge/-lefthook-000000.svg?logo=lefthook&style=flat)](https://lefthook.dev/)
[![Storybook](https://img.shields.io/badge/-Storybook-E00080.svg?logo=storybook&style=flat)](https://storybook.js.org/)

# About
Next.js 構築で使用するボイラーテンプレート

## Tech Stack

| stack | version |
| --- | --- |
| Next.js | 16.3.5 |
| React | 19.2.8 |
| Tailwind/postcss | 4 |
| oxlint | 1.85.0 |
| oxfmt | 0.70.0 |
| lefthook | 2.1.14 |
| Storybook | 10.6.0 |

## Getting Started

ローカル開発:

```bash
pnpm dev
```

URL: [http://localhost:3000](http://localhost:3000)

## Project Structure

```text
/
├── public/             加工なしでそのまま配信される静的ファイル (image etc.)
├── src/
│   ├── api/            ※慣例名。APIクライアント・データ取得関数など
│   ├── app/            ※必須。ファイルがそのままURLになる (App Router / file-based routing)
│   ├── components/     ※慣例名。再利用するUIコンポーネント
│   └── lib/            ※慣例名。ユーティリティ関数・共通ロジック
├── stories/            Storybookのストーリーファイル
├── .storybook/         Storybook設定ファイル (main.ts, preview.tsx)
├── eslint.config.mjs   ESLint設定ファイル
├── lefthook.yml        Git hooks設定 (lefthook)
├── next.config.ts      Next.js設定ファイル
├── postcss.config.mjs  PostCSS設定ファイル (Tailwind CSS)
├── vitest.config.ts    Vitest設定ファイル
├── tsconfig.json       TypeScript設定ファイル
└── package.json        パッケージ情報・スクリプト定義
```

## CLI

| Command | Description |
| --- | --- |
| `pnpm dev` | 開発サーバー起動 |
| `pnpm build` | ビルド |
| `pnpm lint` | リンターを実行 |
| `pnpm lint:fix` | リンターを実行して修正を適用 |
| `pnpm fmt` | フォーマッター |
| `pnpm fmt:fix` | フォーマッターを実行して修正を適用 |
| `pnpm storybook` | Storybookを起動 |
| `pnpm build-storybook` | Storybookをビルド |

## Learn More

- [Next.js Documentation](https://nextjs.org/docs) 
- [Learn Next.js](https://nextjs.org/learn)
- [the Next.js GitHub repository](https://github.com/vercel/next.js)
