# Codex・クラウド環境用のsandbox

Codexとクラウド上の開発環境の使い方を、実際にコードを動かしながら学ぶためのリポジトリ
小さな実験を通じて、Codexへの依頼、ファイルの編集、コマンドの実行、結果の確認用

## pnpmで実行する

Node.jsとpnpmが使える環境で、リポジトリのフォルダーから実行します。

```bash
pnpm install
pnpm start
```

`pnpm install` は依存パッケージを準備するコマンドです。今回は追加の依存パッケージはありません。
`pnpm start` は `package.json` の `scripts.start` に記載した `node hello.js` を実行します。
使用するpnpmのバージョンは `packageManager` に記録しています。
このクラウド環境でも保存できるよう、`pnpm-workspace.yaml` でパッケージの保存先を `.pnpm-store` に指定しています。
