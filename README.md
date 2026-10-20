# 아스타나키즈 이벤트 페이지

매장에서 QR을 찍으면 바로 열리는 휴대폰용 이벤트 안내 페이지입니다. GitHub Pages로 무료 공개합니다.

| 이벤트 | 주소 | QR |
|---|---|---|
| 재방문 돈까스 무한 득템 (2026-10-26~) | https://gnb21c-cmd.github.io/event/donkatsu/ | `qr/donkatsu.png` |

`https://gnb21c-cmd.github.io/event/` 로 들어와도 지금 이벤트로 넘어갑니다.

## 처음 한 번: 페이지 켜기

저장소 **Settings → Pages → Build and deployment**
- Source: **Deploy from a branch**
- Branch: **main** / **/(root)** → Save

1~10분 뒤 위 주소가 열립니다.

## 구성

- `donkatsu/index.html` — 페이지 전체 (디자인·문구·동작이 한 파일)
- `donkatsu/img/` — 홍보 이미지(`poster`), 돈까스 접시(`plate`), 돼지 캐릭터(`pig`), 카카오톡 미리보기(`og.jpg`)
- `index.html` — 저장소 첫 주소를 지금 이벤트로 넘김

## 본 사람 수 (다섯 자리 숫자)

- 무료 집계 서비스 [Abacus](https://jasoncameron.dev/abacus/) 를 씁니다. 이름: `gnb21c-event` / `donkatsu-2026`
- 같은 휴대폰의 같은 브라우저는 한 번만 셉니다 (브라우저 저장소 + 쿠키). 다만 같은 사람이라도 카카오톡 안 브라우저와 휴대폰 기본 브라우저로 각각 열면 두 번, 방문 기록을 지우거나 시크릿 모드면 다시 셉니다.
- 주소 끝에 `?test` 를 붙이면 세지 않고 숫자만 봅니다 (직원 확인용).
- 지금 숫자만 보기: https://abacus.jasoncameron.dev/get/gnb21c-event/donkatsu-2026
- 6개월 동안 아무도 안 열면 기록이 지워지는 무료 서비스입니다.

## 카카오톡 공유

- 지금은 휴대폰 공유 메뉴가 열리고, 거기서 카카오톡을 고릅니다. 공유 메뉴가 없는 브라우저(카카오톡 안 브라우저 등)에서는 링크를 복사합니다.
- 카카오톡 친구 고르기 창이 바로 열리게 하려면: [Kakao Developers](https://developers.kakao.com) 에서 앱을 만들고, 웹 도메인에 `https://gnb21c-cmd.github.io` 를 등록한 뒤, **JavaScript 키**를 `donkatsu/index.html` 의 `KAKAO_JS_KEY` 에 넣습니다. (JavaScript 키는 원래 페이지에 공개되는 값이고, 등록한 도메인에서만 작동합니다.)

## 이벤트를 끝낼 때

페이지를 지우지 말고 "이벤트가 종료되었습니다" 안내로 바꿔 둡니다. 이미 붙은 포스터의 QR을 찍은 사람이 오류 화면을 보지 않게 하기 위해서입니다. 저장소 이름·폴더 이름을 바꾸면 QR 주소가 끊깁니다.
