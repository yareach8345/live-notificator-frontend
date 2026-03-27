# Live Notificator Frontend

## ▶️️ プロジェクト紹介

---
ライブ配信通知システムのフロントエンド

バックエンドからデータを取得して出力し、システムを制御するためのインタフェースを提供する。

### 🗓️ 開発期間
２０２５年４月２１日 ~ ２０２５年７月１０日

### ⚙️ 使用技術
- Nuxt.js
- tailwindcss
- pinia
- SSE

### 🌐 他のサイト
![Static Badge](https://img.shields.io/badge/notion-project-a980f7?logo=notion&logoColor=white&link=https%3A%2F%2Fwww.notion.so%2FLive-Notificator-30fad8559b2d80869161d2083afa5ed7)
![Static Badge](https://img.shields.io/badge/github-backend-red?logo=github&logoColor=white&link=https%3A%2F%2Fgithub.com%2Fyareach8345%2Flive-notificator-backend)
![Static Badge](https://img.shields.io/badge/github-sms-5552ff?logo=github&logoColor=white&link=https%3A%2F%2Fgithub.com%2Fyareach8345%2Flive-notificator-sms)

## 使用方法
### environment variables
```text
BACKEND_BASE_URL="BACKEND_URL"

YOUTUBE_API_KEY="YOUTUBE_API_KEY"
```
| property        | value           |
|-----------------|-----------------|
| API_BASE_URL    | バックエンドのURL      |
| YOUTUBE_API_KEY | youtube API Key |
* ユーチューブの機能は削除する予定、この環境変数も削除対象

## ページ情報
| エンドポイント                               | 説明                         |
|---------------------------------------|----------------------------|
| /                                     | ログインのあとメインページ              |
| /login                                | ログインページ                    |
| /not-valid-user                       | 許可されていないアカウントでログインしたら見える画面 |
| /channels                             | 登録したチャンネルのリスト              |
| /channels/register                    | モニタリング対象にチャンネルを追加          |
| /channels/[platform]/[channelId]      | チャンネル情報ページ                 |
| /channels/[platform]/[channelId]/edit | チャンネル情報変更                  |
| /devices                              | 登録したデバイスのリスト               |
| /devices/register                     | バックエンドからデータを取得するデバイスを追加    |
| /devices/[devideId]                   | デバイスの情報を見る                 |
| /devices/[deviceId]/edit              | デバイスの情報を変更　                |
| /events-view                          | SSEを通してバックエンドから受信したイベントのログ |
