# Ollama チャット

このリポジトリには、ローカルで動作する Ollama モデルと対話できる最小限のウェブページが含まれています。ページでは JavaScript の `fetch` を用いてサーバーからストリーミングで応答を受け取ります。

## 使い方
1. まず `ollama serve` などで Ollama サーバーを起動し、ポート `11434` で待ち受けさせます。
2. `index.html` をブラウザで開きます。スタンドアロンのファイルとして動作するので、そのままダブルクリックしても、任意の Web サーバーで配信してもかまいません。
3. モデルは入力欄横のプルダウンから選択できます。別のサーバーを利用したい場合は、`index.html` のスクリプト冒頭にある `endpoint` 変数を変更してください。
4. 入力欄では `Shift + Enter` で改行ができます。

## 依存関係
- `http://localhost:11434` でアクセス可能なローカルの Ollama サーバー
