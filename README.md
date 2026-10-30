# FlashCast

月面衝突閃光（LIF）の観測を計画するウェブアプリ FlashCast の公開用リポジトリ。

**開く: https://cosmic-nori.github.io/flashcast-app/**

流星群ごとの観測窓、望遠鏡の視野の置き方、検出の期待数、測光標準星の選定、検出した閃光の起源の確率を計算する。日本語と英語を切り替えられる。

このリポジトリには、ブラウザが読むファイルだけを置いている。ソースと設計書は別の非公開リポジトリで管理し、更新のたびにここへ反映する。

- `index.html`: アプリ本体（1 ファイル）。ダウンロードしてブラウザで開いても動く（そのときは月面の高精細なタイルを読めないので、埋め込みの画像で描く）。
- `wac/`: 拡大した月面図と一人称表示に使う月面のタイル。
- `version.json`: このサイトを作ったソースのコミットと日時。

## クレジット

- 月面画像: NASA SVS CGI Moon Kit（LRO LROC WAC）、LROC WAC Global Morphology Mosaic 100 m（USGS Astrogeology / LROC team）。地球の画像: NASA Blue Marble（Visible Earth）。
- 暦: Astronomy Engine 2.1.19（MIT）。3D 表示: three.js 0.160.0（MIT、jsDelivr から読み込む）。
- 標準星: Smith et al. (2002)、Landolt (2009, 2013)、SIMBAD、Gaia DR3。輝星: Yale Bright Star Catalogue。
