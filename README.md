# J.a.M Official Website

架空アイドル J.a.M の公式サイトです。GitHub Pages で公開します。

- `index.html` … 公開サイト
- `admin.html` … 管理画面（NEWS / BLOG / SPECIAL を編集）
- `cms.json` … NEWS / BLOG / SPECIAL の中身。管理画面がここを書き換えます
- `img/` `frag/` `jackets/` … 画像

## 公開の手順

1. このフォルダの中身を、新しいリポジトリ（例：`jam-official`）にそのまま入れる
2. リポジトリの **Settings → Pages** で、Source を「Deploy from a branch」、Branch を `main` / `(root)` にして Save
3. 1〜2分で `https://<ユーザー名>.github.io/<リポジトリ名>/` が公開される

## 管理画面の準備（最初の1回だけ）

1. GitHub の **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**
   - Repository access：**Only select repositories** でこのリポジトリだけを選ぶ
   - Permissions：**Contents** を **Read and write**
   - 有効期限は好みで（切れたら作り直して入れ直す）
2. スマホで `https://<ユーザー名>.github.io/<リポジトリ名>/admin.html` を開く
3. ユーザー名・リポジトリ名・トークンを入れて「保存して接続」
4. ホーム画面に追加しておくと、アプリのように開けます

トークンはその端末のブラウザの中だけに保存されます。端末を手放すときは、管理画面の「設定 → この端末からトークンを消す」を押すか、GitHub 側でトークンを削除してください。

## 使い方

編集して「変更を反映」→ 最後に画面下の「サイトに公開」。
公開すると `cms.json` が更新され、1〜2分でサイトに反映されます。
