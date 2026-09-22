# GitHub Pages（法的文書）

このフォルダを GitHub Pages で公開すると、審査用の固定 URL になります。

## 公開手順

1. このリポジトリを GitHub に作成・push する
2. GitHub → **Settings** → **Pages**
3. **Source**: Deploy from a branch
4. **Branch**: `main`（または `master`） / folder: `/docs`
5. Save 後、数分待つ

## URL 例

リポジトリ名が `Egg`、ユーザー名が `yoshi` の場合:

- トップ: `https://yoshi.github.io/Egg/`
- プライバシーポリシー: `https://yoshi.github.io/Egg/privacy.html`
- 利用規約: `https://yoshi.github.io/Egg/terms.html`

## 公開前に必ず行うこと

- `privacy.html` / `terms.html` の `YOUR_EMAIL@example.com` を実メールに変更する
- ブラウザで両ページが開けることを確認する（ログイン不要）

## アプリへの設定

```text
EXPO_PUBLIC_PRIVACY_POLICY_URL=https://<user>.github.io/<repo>/privacy.html
EXPO_PUBLIC_TERMS_URL=https://<user>.github.io/<repo>/terms.html
```

または `app.json` の `extra.legal` に同じ URL を書く。
