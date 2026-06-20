# Ur Metronome — Legal

iPhone アプリ **Ur Metronome** のプライバシーポリシーと利用規約を公開するためのリポジトリ。
App Store ガイドライン 3.1.2（サブスクリプションの必須開示）に対応する。

GitHub Pages で配信する静的 HTML のみを置く。

## ページ

| ファイル | 公開 URL（Pages 有効後） |
|---|---|
| `index.html` | `https://acer8160.github.io/legal/` |
| `privacy-policy.html` | `https://acer8160.github.io/legal/privacy-policy.html` |
| `terms-of-use.html` | `https://acer8160.github.io/legal/terms-of-use.html` |

## 編集ルール

- 本文の原本（ドラフト）はアプリ本体リポジトリの `docs/legal/*.ja.md`。
  内容を変えるときは原本も合わせて更新する。
- **連絡先は Google フォーム**（公開・ログイン不要）。メールアドレスは公開しない。
  フォーム URL はアプリ本体の `constants/feedback.ts`（ja）と同一。差し替え時は両方更新する。

## デプロイ

`main` ブランチへの push で GitHub Pages が自動反映される（Settings → Pages → Source: `main` / root）。
`.nojekyll` を置いているため Jekyll ビルドは行われず、HTML がそのまま配信される。
