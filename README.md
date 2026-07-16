# tiktok-sandbox-policy

TikTok Developer Sandbox申請用のプライバシーポリシー静的ページ。
GitHub Pagesでホスティングして、TikTok for DevelopersアプリのSandbox設定画面にURLを登録する。

## セットアップ手順

1. GitHubで新規リポジトリを作成(例: `tiktok-sandbox-policy`)。Public推奨(GitHub Pages無料枠はPublicリポジトリが前提)。

2. このディレクトリの中身をpush

   ```bash
   git remote add origin https://github.com/<あなたのユーザー名>/tiktok-sandbox-policy.git
   git add -A
   git commit -m "Add privacy policy page for TikTok sandbox"
   git branch -M main
   git push -u origin main
   ```

3. GitHubのリポジトリ設定 → Pages で、
   - Source: `Deploy from a branch`
   - Branch: `main` / `root`
   を選択して保存。

4. 数分後、以下のURLで公開される:

   ```
   https://<あなたのユーザー名>.github.io/tiktok-sandbox-policy/
   ```

5. TikTok for Developers のアプリ設定で、以下のようにURLを登録する:

   | 項目 | URL |
   |---|---|
   | Web/Desktop URL(公式サイト) | `https://<あなたのユーザー名>.github.io/tiktok-sandbox-policy/` |
   | Privacy Policy URL | `https://<あなたのユーザー名>.github.io/tiktok-sandbox-policy/privacy.html` |
   | Terms of Service URL | `https://<あなたのユーザー名>.github.io/tiktok-sandbox-policy/terms.html` |

## ページ構成

- `index.html` … アプリの簡単な紹介ページ(Web/Desktop URLとして登録)
- `privacy.html` … プライバシーポリシー
- `terms.html` … 利用規約

## 注意

- `index.html` の内容は実際に取得するデータ・スコープと一致させること(Sandboxでも記載内容の正確性が審査対象になり得る)。
- 本番申請(Production)に進む場合は、利用規約(Terms of Service)ページも別途用意することを推奨。
