# Live Notificator Frontend

일본어 문서는 아래 파일음 참고해주세요.

日本語の文書はこちらのファイルをご覧ください。
[日本語の文書](README.md)

## ▶️️ 프로젝트 소개

---
라이브 방송 통지 시스템의 프론트엔드

백엔드에서 부터 데이터를 가져와 출력하고, 시스템을 제어하기 위한 인터페이스를 제공

### 🗓️ 개발기간
2025년 4월 21일 ~ 2025년 7월 10일

### ⚙️ 사용기술
- Nuxt.js
- tailwindcss
- pinia
- SSE

### 🌐 더보기
![Static Badge](https://img.shields.io/badge/notion-project-a980f7?logo=notion&logoColor=white&link=https%3A%2F%2Fwww.notion.so%2FLive-Notificator-30fad8559b2d80869161d2083afa5ed7)
![Static Badge](https://img.shields.io/badge/github-backend-red?logo=github&logoColor=white&link=https%3A%2F%2Fgithub.com%2Fyareach8345%2Flive-notificator-backend)
![Static Badge](https://img.shields.io/badge/github-sms-5552ff?logo=github&logoColor=white&link=https%3A%2F%2Fgithub.com%2Fyareach8345%2Flive-notificator-sms)

## 사용법
### environment variables
```text
BACKEND_BASE_URL="BACKEND_URL"

YOUTUBE_API_KEY="YOUTUBE_API_KEY"
```
| property        | value           |
|-----------------|-----------------|
| API_BASE_URL    | 백엔드 url         |
| YOUTUBE_API_KEY | youtube API Key |
* 유튜브 기능은 삭제예정이며, 환경변수 또한 삭제 대상입니다.

## 페이지
| 엔드포인트                                 | 설명                           |
|---------------------------------------|------------------------------|
| /                                     | 로그인 후의 메인페이지                 |
| /login                                | 로그인 페이지                      |
| /not-valid-user                       | 허가되지 않은 계정으로 로그인할 시 가게되는 페이지 |
| /channels                             | 등록한 채널 리스트                   |
| /channels/register                    | 모니터링 대상인 채널을 추가              |
| /channels/[platform]/[channelId]      | 채널 정보 보기                     |
| /channels/[platform]/[channelId]/edit | 채널 정보 수정                     |
| /devices                              | 등록된 디바이스 목록                  |
| /devices/register                     | 백엔드에서 데이터를 취득할 디바이스 추가       |
| /devices/[devideId]                   | 디바이스 정보 보기                   |
| /devices/[deviceId]/edit              | 디바이스 정보 수정                   |
| /events-view                          | SSE를 통해 받은 데이터 보기            |
