# kurenkai-site

旭区連合自治会町内会連絡協議会 定例会資料の公開ページ。

- このリポジトリには、**自動生成された HTML と CSS だけ**を置きます。
- 会議の文字起こし・役員会向け資料（補足つき要約）・PDF 実体・中間データは置きません。
  `.gitignore` が allowlist 方式になっており、許可したファイル以外は登録されません。
- 生成は別フォルダの道具（`../kurenkai`）が行います。ここは置き場所です。

## 公開設定

GitHub Pages の公開元は **このリポジトリの `main` ブランチ直下（`/`）** です。

## 更新のしかた

1. Claude に `/kurenkai` と伝えて月別ページを作る
2. VS Code のソース管理ビューで内容を確認する
3. 「↑」（変更の同期）を押す → GitHub Pages が更新される

## 公開前の確認

push する前に、登録されるファイルが想定どおりか確認します。

```
git ls-files
```

出てきてよいのは次のものだけです。

- `.gitignore`
- `README.md`
- `index.html`
- `assets/style.css`
- `{yyyymm}/index.html`
