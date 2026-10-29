# Joli Skin Clinic｜たるみ設計カウンセリング 動画広告 完成案

社内共有用の資料です。GitHub Pages で URL を発行して閲覧するためのファイル一式です。

- 本文は `index.html`（ブラウザで見る用）と `plan.md`（GitHub 上でそのまま読む用）で同じ内容です。
- 書き出した動画（BGM入り・ナレーションなし、A〜Eの5案）は `videos.html` で再生できます。動画ファイルは `動画/` にあります。
- 追加2案（D・E）の構成は `plan-de.html`（GitHub 上で読むなら `plan-de.md`）にあります。
- 検索エンジンに載らないよう、`index.html` に `noindex` を、`robots.txt` にクロール拒否を入れています。
- 元の資料は Claude Docs の完成案（2026年10月29日版）です。

## 公開手順（GitHub Pages）

1. GitHub で新しいリポジトリを作成する（例：`joli-tarumi-video-plan`）。
2. 「Add file」→「Upload files」で、このフォルダの中身（`index.html`、`videos.html`、`plan-de.html`、`plan.md`、`plan-de.md`、`動画` フォルダ、`img` フォルダ、`robots.txt`、`README.md`、`.nojekyll`）をドラッグしてアップロードし、「Commit changes」。
3. リポジトリの「Settings」→「Pages」を開き、「Source」を「Deploy from a branch」、Branch を `main` / `/(root)` にして「Save」。
4. 1〜2分後、同じ画面に表示される URL（`https://<ユーザー名>.github.io/<リポジトリ名>/`）で閲覧できます。

既存のリポジトリに追加する場合は、フォルダごと（例：`joli-tarumi/`）アップロードすると `https://<ユーザー名>.github.io/<リポジトリ名>/joli-tarumi/` で見られます。

## 注意

- 無料プランの GitHub Pages は、リポジトリを Public（公開）にする必要があります。広告費・Lead 数などの数字、院への確認事項、配信前の動画を含むため、URL を知っている人以外にも見える状態になる点に注意してください。
- 公開せずに共有するだけなら、Private リポジトリにして相手を招待し、`plan.md` を GitHub 上で読んでもらう方法もあります。
- 公開をやめるときは、Settings → Pages で無効にするか、リポジトリを削除します。

## ファイル構成

```
index.html          ページ本体（スマホ・タブレット・PC 対応）
videos.html         動画5案の再生ページ（BGM入り・ナレーションなし）
plan-de.html        追加2案（D・E）の構成
plan.md             同じ内容の Markdown 版（GitHub 上で表示される）
plan-de.md          追加2案の Markdown 版
動画/               A〜E の 9:16 と 4:5（mp4、計10本）
img/age-leads.svg   年齢区分別 Lead のグラフ（plan.md 用）
img/poster_*.jpg    動画のサムネイル（videos.html 用）
img/strip_*.jpg     D・E の各カットの静止画（plan-de 用）
robots.txt          検索エンジンのクロール拒否
.nojekyll           GitHub Pages の自動変換を止める設定
```
