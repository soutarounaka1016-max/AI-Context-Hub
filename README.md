# AI Context Hub

別AIへ渡すユーザーコンテキストを、ボタン1つでコピーするための個人用ツールです。

## 重要な設計

このリポジトリは公開されても個人データが漏れないように、**コンテキスト本文をGitHubへ保存しません**。

- GitHub: UIコードだけ
- 個人コンテキスト: 利用端末のブラウザ `localStorage` に保存
- 初回のみ starter JSON を読み込む
- 以後は QUICK / STANDARD / BUSINESS / STUDY / FULL を1タップでコピー

APIキー、パスワード、連絡先、正確な住所などの秘密情報は保存しないでください。

## 使い方

1. GitHub Pagesでこの `index.html` を公開する。
2. ページを開く。
3. 「初期データを読み込む」から ChatGPT が作成した starter JSON を選ぶ。
4. 以後、用途に応じてコピーボタンを押すだけ。

同じデータを別端末でも使う場合は、「バックアップを書き出す」でJSONを保存し、別端末で読み込めます。

## GitHub Pages

Repository Settings → Pages から `main` ブランチのルートを公開対象に設定してください。

## Privacy

ブラウザのデータを削除すると、localStorage内のコンテキストも消えることがあります。必要ならバックアップJSONを保管してください。
