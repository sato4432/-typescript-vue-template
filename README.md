# Vue + TypeScript テンプレート

このテンプレートは、Vue 3とTypeScriptを使用した開発を始めるための環境を提供します。
厳格なコード品質を確保するため、ESLintとPrettierを利用した厳しめのコード品質チェック機構が組み込まれています。

## 特徴

- **Vue 3**: 最新のVueフレームワークを使用
- **TypeScript**: 強力な型システムによる安全なコーディング
- **Vite**: 高速な開発サーバーとビルドツール
- **ESLint**: 厳格なコード品質チェック
  - Vue推奨ルール
  - TypeScript厳格ルール
  - 共通的なベストプラクティス
- **Prettier**: 一貫したコードフォーマット
- **コマンド**: 開発、ビルド、型チェック、リント、フォーマットなどの便利なコマンド

## コード品質について

このテンプレートでは、以下のような厳格なコード品質ルールを採用しています：

- TypeScriptの厳格モードを有効化
- 未使用変数・パラメータの禁止
- `any`型の使用禁止
- 関数の戻り値の型を明示的に指定
- Vue関連のベストプラクティスを強制
- 一貫したコードスタイルを確保

## 推奨IDE設定

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (Veturは無効化してください)

## セットアップ

```sh
npm install
```

### 開発サーバー起動

```sh
npm run dev
```

### 型チェックとビルド

```sh
npm run build
```

### コード品質チェック

```sh
# リントチェック（エラー検出のみ）
npm run lint:check

# リント実行（自動修正あり）
npm run lint

# フォーマットチェック（エラー検出のみ）
npm run format:check

# フォーマット実行（自動修正あり）
npm run format
```

## 参考リンク

- [Vue公式ドキュメント](https://vuejs.org/)
- [Vite公式ドキュメント](https://vitejs.dev/)
- [TypeScript公式ドキュメント](https://www.typescriptlang.org/)
- [ESLint公式ドキュメント](https://eslint.org/)
- [Prettier公式ドキュメント](https://prettier.io/)

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).
