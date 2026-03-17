# 都市爆破アプリ

このリポジトリは共同開発練習用です。
Docker, Github, ClaudeAIなどの練習を目的としています。

## 概要

このREADME.mdは開発者向けです。
このアプリは共同開発練習用を目的として開発されています。現実世界の事故や事件と一切の関連がありません。

## 使用技術

- Ruby on Rails 8
- hotwire(Turbo + Stimulus)
- Importmap(ビルドツールなし)
- bundler
- PostgreSQL
- デプロイ: Render.com
- テスト: Minitest

## 開発環境

- Ruby: 3.3.6
- Rails: 8.1.2
- DataBase: PostgreSQL 17.6
- bundler 2.7.2
- tailwindcss-rails: 4.4.0

## セットアップ手順

- リポジトリをクローン
- Docker起動
- イメージをビルド ($ docker compose build)
- 開発サーバー起動($ docker compose up)

## その他

- webコンテナを起動($ docker compose exec web bash)
- dbコンテナを起動($ docker compose exec web bash)
- コンテナを抜ける($ exit)
- パッケージをインストール($ docker compose exec web bundle install)
- db作成($ docker compose exec web rails db:create)
- マイグレーション($ docker compose exec web rails db:migrate)
- cssを手動リロード(webサーバーがフォアグラウンドで起動した状態で$ bin/rails tailwindcss:build)

## 機能一覧

- ユーザー機能
- 都市爆破機能
- 爆破予告の投稿機能
- 他

# デプロイ

https://group-dev-test1.onrender.com/

# ER図

https://docs.google.com/spreadsheets/d/16cRnw4BspA6Wa4jGW1-asSGCAHDCItwtfKinyL2nabk/edit?gid=0#gid=0
