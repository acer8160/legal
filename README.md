# Legal

iPhone アプリのプライバシーポリシーと利用規約を公開するためのリポジトリ。
App Store ガイドライン 3.1.2（サブスクリプションの必須開示）に対応する。

GitHub Pages で配信する静的 HTML のみを置く。

- **Your Metronome**: ルート直下（歴史的経緯。移動・リネーム禁止 — 公開済みアプリが URL を直接参照している）
- **関所ロック（Sekisho Lock）**: `sekisho-lock/` 配下

## ページ（Your Metronome）

| ファイル | 公開 URL（Pages 有効後） |
|---|---|
| `index.html` | `https://acer8160.github.io/legal/` |
| `privacy-policy.html`（日本語） | `https://acer8160.github.io/legal/privacy-policy.html` |
| `terms-of-use.html`（日本語） | `https://acer8160.github.io/legal/terms-of-use.html` |
| `privacy-policy.en.html`（English） | `https://acer8160.github.io/legal/privacy-policy.en.html` |
| `terms-of-use.en.html`（English） | `https://acer8160.github.io/legal/terms-of-use.en.html` |

## ページ（関所ロック / Sekisho Lock）

| ファイル | 公開 URL |
|---|---|
| `sekisho-lock/index.html` | `https://acer8160.github.io/legal/sekisho-lock/` |
| `sekisho-lock/privacy-policy.html`（日本語） | `https://acer8160.github.io/legal/sekisho-lock/privacy-policy.html` |
| `sekisho-lock/terms-of-use.html`（日本語） | `https://acer8160.github.io/legal/sekisho-lock/terms-of-use.html` |
| `sekisho-lock/privacy-policy.en.html`（English） | `https://acer8160.github.io/legal/sekisho-lock/privacy-policy.en.html` |
| `sekisho-lock/terms-of-use.en.html`（English） | `https://acer8160.github.io/legal/sekisho-lock/terms-of-use.en.html` |

- 連絡先は Google フォーム（日英共通・ログイン不要）。メールアドレスは公開しない。
- 原本 Markdown はアプリ本体リポジトリ（App_lock）の `docs/legal/` に置く運用（内容変更時は原本と HTML の両方を更新する）。

## 編集ルール

- 本文の原本（ドラフト）はアプリ本体リポジトリの `docs/legal/*.ja.md` / `*.en.md`。
  内容を変えるときは原本も合わせて更新する（ja/en 両方）。
- アプリ内のリンクは表示言語で ja/en を出し分ける（`constants/paywall.ts` が locale 別 URL を持つ）。
- **連絡先は Google フォーム**（公開・ログイン不要）。メールアドレスは公開しない。
  ja フォーム / en フォームの URL はアプリ本体の `constants/feedback.ts` と同一。差し替え時は両方更新する。

## デプロイ

`main` ブランチへの push で GitHub Pages が自動反映される（Settings → Pages → Source: `main` / root）。
`.nojekyll` を置いているため Jekyll ビルドは行われず、HTML がそのまま配信される。
