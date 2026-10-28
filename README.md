# 全自動AIテックラボ（公式サイト）

YouTube チャンネル「全自動AIテックラボ」（[@auto-ai-techlab](https://www.youtube.com/@auto-ai-techlab)）のサイトです。

- 公開URL：https://autotoolspublisher-ui.github.io/auto-ai-techlab/
- 内容：チャンネルの紹介、各回の動画の一覧と「試してわかったこと」、各回の個別ページ（`videos/epNNN/`）、プライバシーポリシー（`privacy.html`）
- このチャンネルとサイトは、AI（Claude）が制作・運営しています。公開の判断は運営（人間）が行います

## このリポジトリについて

- このリポジトリのファイルは、運営のPCの作業フォルダにある元データ（`site/src/`）から、スクリプト（`site/tools/build_site.py`）で作ったものです。**ここを直接編集しないでください**（次の更新で上書きされます）
- 更新：動画の公開日（月・水・金 18:00）の夜に、予定の作業が新しい回を足して push します
- 公開：GitHub Pages（`main` ブランチのルート）

## ファイル

| ファイル | 内容 |
| --- | --- |
| `index.html` | トップページ（チャンネルの紹介と動画の一覧） |
| `videos/epNNN/index.html` | 各回の個別ページ |
| `privacy.html` | プライバシーポリシー |
| `sitemap.xml` | サイトマップ（Google Search Console に登録済み） |
| `llms.txt` | AI 向けのサイトの説明 |
| `favicon.svg` | ファビコン |
| `.nojekyll` | GitHub Pages の Jekyll の処理を止める |

## Google アナリティクス（2026-10-28 運営の決定で追加）

- 測定 ID：`G-WP0CG915CL`
- すべてのページの `<head>` の先頭（`<meta charset="utf-8">` の直後）に、Google アナリティクスのタグ（gtag.js）を入れている
- 元はテンプレート（`site/src/index.template.html`・`episode.template.html`・`privacy.template.html`）。新しい回のページにも自動で入る。このリポジトリの HTML だけを直すと、次の更新でタグが消えるので、変えるときは必ずテンプレートを直す
- プライバシーポリシー（`privacy.html`、2026-10-28 更新）に、Google アナリティクスを使うこと・Cookie を使うこと・止め方（[Google アナリティクス オプトアウト アドオン](https://tools.google.com/dlpage/gaoptout?hl=ja)）を書いている
- 個人を特定する情報（名前・メールアドレスなど）は送らない

## ライセンス

- サイトの文章・構成：© 全自動AIテックラボ
- 動画のサムネイルは YouTube から表示しています（このリポジトリには置いていません）
- 音声：VOICEVOX:春日部つむぎ／立ち絵：春日部つくし（春日部つむぎ公式立ち絵素材）。素材はこのリポジトリに含みません
