# Joli Skin Clinic｜たるみ設計カウンセリング 動画広告 完成案

社内共有用の資料です。GitHub Pages で URL を発行して閲覧するためのファイル一式です。

- 本文は `index.html`（ブラウザで見る用）と `plan.md`（GitHub 上でそのまま読む用）で同じ内容です。
- 書き出した動画（BGM入り・ナレーションなし、A〜Iの9案）は `videos.html` で再生できます。動画ファイル（mp4）はページと同じ階層にあります。
- 追加案の構成は `plan-de.html`（D・E）、`plan-fg.html`（F・G）、`plan-hi.html`（H・I）にあります（GitHub 上で読むなら `.md`）。
- 検索エンジンに載らないよう、`index.html` に `noindex` を、`robots.txt` にクロール拒否を入れています。
- 元の資料は Claude Docs の完成案（2026年11月2日時点）です。

## 公開手順（GitHub Pages）

今の公開先は `ibukinegishi-spec/joli_clinic` リポジトリの一番上の階層で、URL は https://ibukinegishi-spec.github.io/joli_clinic/ です。

1. `stage_upload.py` を実行すると、GitHub にあるものと比べて新しいか変わったファイルだけが `共有用/GitHubに上げる/` に、`1_動画` と `2_ページ` に分かれて入ります。
2. GitHub のリポジトリのトップで「Add file」→「Upload files」を開き、`1_動画` の中身（mp4）をドラッグして「Commit changes」。
3. もう一度「Upload files」を開き、`2_ページ` の中身（html・md・`img` フォルダなど）をドラッグして「Commit changes」。
4. 1〜2分で公開ページに反映されます（Settings → Pages は設定済み）。

ブラウザからのアップロードは1ファイル25MBまで。mp4 はどれも10MB以下です。2回に分けるのは、1回のアップロードが重くなりすぎないようにするためです。

## 注意

- 無料プランの GitHub Pages は、リポジトリを Public（公開）にする必要があります。広告費・Lead 数などの数字、院への確認事項、配信前の動画を含むため、URL を知っている人以外にも見える状態になる点に注意してください。
- 公開せずに共有するだけなら、Private リポジトリにして相手を招待し、`plan.md` を GitHub 上で読んでもらう方法もあります。
- 公開をやめるときは、Settings → Pages で無効にするか、リポジトリを削除します。

## ファイル構成

```
index.html          ページ本体（スマホ・タブレット・PC 対応）
videos.html         動画9案の再生ページ（BGM入り・ナレーションなし）
plan-de.html        追加2案（D・E）の構成
plan-fg.html        追加2案（F・G）の構成
plan-hi.html        追加2案（H・I）の構成（2本とも静止画版を制作）
plan.md             同じ内容の Markdown 版（GitHub 上で表示される）
plan-de.md          追加2案（D・E）の Markdown 版
plan-fg.md          追加2案（F・G）の Markdown 版
plan-hi.md          追加2案（H・I）の Markdown 版
*.mp4               A〜I の 9:16 と 4:5（計18本。GitHub に上げた形に合わせ、フォルダに分けない）
img/age-leads.svg   年齢区分別 Lead のグラフ（plan.md 用）
img/poster_*.jpg    動画のサムネイル（videos.html 用）
img/strip_*.jpg     D〜I の各カットの静止画（追加案のページ用）
robots.txt          検索エンジンのクロール拒否
.nojekyll           GitHub Pages の自動変換を止める設定
```
