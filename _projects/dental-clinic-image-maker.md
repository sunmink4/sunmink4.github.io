---
title: 치과 이미지 메이커
tagline: 치과 장면 프롬프트를 조립해 Gemini · ChatGPT로 그림과 영상을 만들어 주는 Windows 앱
repository: sunmink4/dental-clinic-image-maker
icon: 🦷
order: 1
tags: [Windows, WPF, Gemini, ChatGPT, API 요금 없음]
downloads:
  - match: '-win-x64\.exe$'
    label: ⬇ 다운로드
    sub: 단일 실행 파일 (권장)
    primary: true
  - match: '-win-x64-framework-dependent\.exe$'
    label: 경량판 받기
    sub: .NET 8 데스크톱 런타임 필요
---

## 소개

치과 장면용 프롬프트를 골라 조립한 뒤, **로그인된 Gemini · ChatGPT 웹 화면**을 앱 안의 브라우저로 대신 조작해서 그림과 영상을 받아 옵니다.

API를 쓰지 않으므로 지금 쓰는 구독 외에 **추가 요금이 들지 않습니다.**

## 기능

- **장면 프리셋** — 실제 사용 기록에서 뽑은 치과 장면(진료 의자, 의사 · 위생사, 환자, 치식 차트 등)
- **화풍 · 비율 선택**, 치과 규칙 체크박스를 프롬프트 끝에 자동으로 붙임
- **참고 이미지 첨부** — 결과의 **참고로** 버튼을 누르면 다음 요청에 바로 첨부
- **수정 요청 칩** — 줌아웃 30%, 탑뷰 등을 눌러 같은 채팅에서 이어서 수정
- **대기열** — 여러 건을 쌓아 두고 한 번에 실행. 연속 3번 실패하거나 한도 문구가 보이면 자동으로 멈춤
- 영상 생성(Gemini)
- 결과는 `저장 폴더\yyyyMMdd\이름.png` 로 날짜별 저장

## 쓰는 법

1. 처음 한 번은 오른쪽 브라우저에서 Gemini(구글)와 ChatGPT에 로그인합니다. 로그인은 다음 실행에도 유지됩니다.
2. 타이틀바에서 Gemini 또는 ChatGPT를 고릅니다. 영상은 Gemini만 됩니다.
3. 장면 프리셋, 화풍, 비율을 고르고 내용을 적습니다.
4. 필요하면 참고 이미지를 첨부하고 **생성**을 누릅니다.

여러 건은 JSON으로도 불러올 수 있습니다.

```json
[{"name":"chair_idle","prompt":"...","provider":"Gemini","kind":"Image","newChat":true,"references":["raw/chair.png"]}]
```

## 설치 방법

받은 exe를 실행하면 됩니다. 따로 설치할 것은 없습니다.

- **다운로드 (권장)** — .NET 런타임까지 들어 있는 단일 실행 파일입니다.
- **경량판** — 크기가 작은 대신 PC에 [.NET 8 데스크톱 런타임](https://dotnet.microsoft.com/download/dotnet/8.0)이 설치되어 있어야 합니다.

Windows가 "PC 보호" 창을 띄우면 **추가 정보 → 실행**을 누르세요.

## 사이트 화면이 바뀌어 안 될 때

자동 조작은 CSS 선택자로 합니다. 왼쪽 아래 **선택자 설정 열기** 버튼으로 `sites.json`을 열어 고친 뒤 앱을 다시 켜면 됩니다.

## 필요 환경

- Windows 10 / 11 (64비트)
- [Microsoft Edge WebView2 런타임](https://developer.microsoft.com/microsoft-edge/webview2/) (Windows 11과 최신 Windows 10에는 기본 설치)
- Gemini 또는 ChatGPT 계정, 인터넷 연결
