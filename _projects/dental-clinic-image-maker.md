---
title: 치과 이미지 메이커
tagline: 치과 장면 프롬프트를 조립해 Gemini · ChatGPT로 그림과 영상을 만들어 주는 Windows 앱
repository: sunmink4/dental-clinic-image-maker
icon: 🦷
order: 1
tags: [Windows, WPF, Gemini, ChatGPT, API 요금 없음]
downloads:
  - match: '-win-Setup\.exe$'
    label: ⬇ 설치판 받기
    sub: 바로가기 · 자동 업데이트 (권장)
    primary: true
  - match: '-win-x64\.exe$'
    label: 설치 없이 실행
    sub: 단일 실행 파일
    beside_primary: true
  - match: '-win-x64-framework-dependent\.exe$'
    label: 경량판 받기
    sub: .NET 8 데스크톱 런타임 필요
---

## 소개

치과 장면용 프롬프트를 골라 조립한 뒤, **로그인된 Gemini · ChatGPT 웹 화면**을 앱 안의 브라우저로 대신 조작해서 그림과 영상을 받아 옵니다.
치과 블로그 · 카드뉴스 · 웹툰 · 게임에 쓸 진료 장면을, 프롬프트를 처음부터 쓰지 않고 칸을 골라 만들 수 있습니다.

API를 쓰지 않으므로 지금 쓰는 구독 외에 **추가 요금이 들지 않습니다.**

## 이런 그림을 만들 수 있습니다

아래는 모두 이 앱으로 만든 그림입니다. 화풍 · 구도 · 인물 · 진료 상황을 칸에서 고르면 그에 맞는 프롬프트가 만들어집니다.

<div class="gallery">
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/photo-wide.jpg' | relative_url }}" alt="실사 진료실 와이드 장면" loading="lazy"><figcaption>실사 다큐 사진 · 진료실 와이드</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/webtoon-pastel.jpg' | relative_url }}" alt="파스텔 웹툰 진료 장면" loading="lazy"><figcaption>웹툰 · 수채 파스텔</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/photo-closeup.jpg' | relative_url }}" alt="실사 구강 검진 클로즈업" loading="lazy"><figcaption>실사 · 검진 클로즈업</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/illust-inset.jpg' | relative_url }}" alt="입안 확대 컷이 들어간 일러스트" loading="lazy"><figcaption>입안 확대 컷 함께 (충치 · 금 인레이)</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/topview-inset.jpg' | relative_url }}" alt="탑뷰 구도의 진료 장면" loading="lazy"><figcaption>위에서 내려다본 구도</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/webtoon-cute.jpg' | relative_url }}" alt="밝은 웹툰풍 거울 확인 장면" loading="lazy"><figcaption>웹툰 · 진료 후 거울 확인</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/photo-inset.jpg' | relative_url }}" alt="입 헹구는 환자와 치아 확대 사진" loading="lazy"><figcaption>실사 · 헹굼 + 치아 확대</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/semireal-macro.jpg' | relative_url }}" alt="반실사 충치 치료 장면" loading="lazy"><figcaption>반실사 · 금 인레이 확대 컷</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/illust-soft.jpg' | relative_url }}" alt="부드러운 일러스트 진료 장면" loading="lazy"><figcaption>일러스트 · 의사와 위생사</figcaption></figure>
</div>

## 앱 화면

<img class="screenshot" src="{{ '/assets/images/dental-clinic-image-maker/app.jpg' | relative_url }}" alt="치과 이미지 메이커 화면 — 왼쪽에 장면 · 화풍 · 인물 설정, 오른쪽에 Gemini 브라우저">
<p class="caption">왼쪽에서 장면과 인물을 고르고, 오른쪽 브라우저(Gemini · ChatGPT)가 그림을 받아 옵니다.</p>

## 고를 수 있는 것

칸마다 **예제 그림 카드**가 있어서, 고르기 전에 어떤 모습인지 보고 고를 수 있습니다. 색만 다른 선택지(가운 · 스크럽 · 체어 색)는 색 견본으로 보여 줍니다.

<div class="option-grid">
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/gender.f20.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>20대 여성 의사</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/hair.f_wavy.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>웨이브 헤어</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/coat.mandarin.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>차이나 칼라 가운</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/coat.surgical.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>일회용 수술 가운</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/acc.loupe.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>루페</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/view.ots_faceless.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>어깨 너머 시점</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/patient.child_f.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>어린이 환자</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/patient.grandma.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>할머니 환자</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/phair.perm.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>뽀글 파마</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/poutfit.uniform.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>교복</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/pcover.drape.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>소공포 + bib</figcaption></figure>
  <figure><img src="{{ '/assets/images/dental-clinic-image-maker/options/situ.rinse.jpg' | relative_url }}" alt="" loading="lazy"><figcaption>입 헹구기</figcaption></figure>
</div>

- **장면 프리셋** — 실사 진료 와이드, 얼굴 클로즈업, 구강 매크로(금 인레이), 환자 시점 로우앵글, 탑다운, 의사 뒤 하이앵글, 웹툰 입안 클로즈업, 웹툰 다음 컷 등
- **화풍 10가지** — 한국 웹툰(게임 에셋), 로맨스 · 일상 개그 · 힐링 수채 · 반실사 드라마 · 스릴러 · SD 꼬마 · 흑백 펜선 웹툰, 실사 다큐 사진, 디지털 페인팅
- **치과의사(주인공)** — 성별 · 나이, 헤어, 가운 종류와 색, 스크럽 색, 마스크, 안경 · 루페 · 청진기 같은 장신구
- **치과위생사** — 성별 · 나이, 헤어, 복장, 마스크, 장신구
- **환자** — 어린이부터 할머니 · 할아버지까지, 헤어, 옷, bib · 소공포, 표정(편안함 · 긴장 · 겁먹음 등)
- **진료 상황 · 치료** — 접수, 체어 안내, 파노라마 엑스레이, 마취, 스케일링, 충치 제거, 레진 충전, 신경 치료, 발치, 임플란트, 헹굼, 거울 확인 등
- **입안 상태** — 충치, 깊은 충치, 금 인레이, 레진, 아말감, 교정 장치, 치석, 건강한 치아 · 치료할 치아 위치
- **체어 · 카메라** — 체어 색 · 기울기, 시점(의사 · 환자 · 어깨 너머), 앵글, 샷 크기, 렌즈, 영상의 카메라 움직임
- **비율 선택**, 치과 규칙 체크박스(글자 · 로고 빼기 등)를 프롬프트 끝에 자동으로 붙임

## 그 밖의 기능

- **참고 이미지 첨부** — 결과의 **참고로** 버튼을 누르면 다음 요청에 바로 첨부. 붙여넣기도 됩니다
- **수정 요청 칩** — 줌아웃 30%, 탑뷰로, 실사로 · 웹툰 컷으로 바꾸기, 자막 · 로고 빼기 등을 눌러 같은 채팅에서 이어서 수정
- **대기열** — 여러 건을 쌓아 두고 한 번에 실행. 연속 3번 실패하거나 한도 문구가 보이면 자동으로 멈춤
- **영상 생성**(Gemini) — 카메라 움직임까지 골라서
- 결과는 `저장 폴더\yyyyMMdd\이름.png` 로 날짜별 저장

## 쓰는 법

1. 처음 한 번은 오른쪽 브라우저에서 Gemini(구글)와 ChatGPT에 로그인합니다. 로그인은 다음 실행에도 유지됩니다.
2. 타이틀바에서 Gemini 또는 ChatGPT를 고릅니다. 영상은 Gemini만 됩니다.
3. 장면 프리셋, 화풍, 비율, 인물 · 상황 칸을 고르고 내용을 적습니다.
4. 필요하면 참고 이미지를 첨부하고 **생성**을 누릅니다.

여러 건은 JSON으로도 불러올 수 있습니다.

```json
[{"name":"chair_idle","prompt":"...","provider":"Gemini","kind":"Image","newChat":true,"references":["raw/chair.png"]}]
```

## 설치 방법

- **설치판 받기 (권장)** — 받은 `Setup.exe`를 실행하면 바로 설치되고 시작 메뉴 · 바탕화면에 바로가기가 생깁니다. 앱을 켤 때 새 버전이 있으면 알려 주고, 누르면 알아서 업데이트합니다.
- **설치 없이 실행** — .NET 런타임까지 들어 있는 단일 실행 파일입니다. 받은 exe를 바로 실행합니다(업데이트는 새로 받아야 합니다).
- **경량판** — 크기가 작은 대신 PC에 [.NET 8 데스크톱 런타임](https://dotnet.microsoft.com/download/dotnet/8.0)이 설치되어 있어야 합니다.

Windows가 "PC 보호" 창을 띄우면 **추가 정보 → 실행**을 누르세요.

## 사이트 화면이 바뀌어 안 될 때

자동 조작은 CSS 선택자로 합니다. 왼쪽 아래 **선택자 설정 열기** 버튼으로 `sites.json`을 열어 고친 뒤 앱을 다시 켜면 됩니다.

## 필요 환경

- Windows 10 / 11 (64비트)
- [Microsoft Edge WebView2 런타임](https://developer.microsoft.com/microsoft-edge/webview2/) (Windows 11과 최신 Windows 10에는 기본 설치)
- Gemini 또는 ChatGPT 계정, 인터넷 연결
