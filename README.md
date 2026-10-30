# 지도 테스트

Google Maps Platform으로 만든 **여행 동선 플래너**입니다. 빌드 없이 `index.html`을 브라우저로 열면 됩니다.

여행 지역과 가고 싶은 장소, 숙소, 여행 시작일을 정하면 영업시간·식사 시간·이동 시간을 반영해 날짜별 최적 방문 순서를 추천합니다.

## 실행 전 준비

`config.example.js`를 `config.js`로 복사한 뒤, 본인의 Google Maps API 키를 넣으세요.
`config.js`는 `.gitignore`에 들어 있어 깃에 올라가지 않습니다.
Google Cloud 콘솔에서 아래 API를 켜야 합니다.

- Maps JavaScript API
- Places API (New)
- Routes API

> API 키는 저장소에 올리지 말고, 키에 HTTP 리퍼러(허용 도메인) 제한을 걸어 두세요.

## 알려진 제한

- Google 경로 서비스는 한국에서 도보·자동차·대중교통 경로를 제공하지 않아, 한국 지역은 직선거리 기반 추정 이동 시간을 씁니다.
- 대중교통은 일부 지역에서 경로를 받지 못해 추정값으로 대체됩니다.
