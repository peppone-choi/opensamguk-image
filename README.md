# OpenSamguk Image Assets

오픈삼국 정적 이미지 에셋 저장소입니다.

이 저장소는 게임/아이콘 리소스를 분리 관리하기 위한 용도이며,
앱 본체 저장소(`opensamguk`)와 배포 저장소(`opensamguk-deploy`)와 독립적으로 운영됩니다.

## 디렉터리 구조

- `icons/` : 장수 초상화 등 아이콘 이미지
- `game/` : 지도, 국기, 이벤트 아이콘, 병종/도시 관련 이미지
- `hook/` : 기존 레거시 운영용 스크립트(호환 목적 보관)

## CDN 사용

기본 CDN (jsDelivr):

`https://cdn.jsdelivr.net/gh/peppone-choi/opensamguk-image@master/`

예시:

- 초상화: `https://cdn.jsdelivr.net/gh/peppone-choi/opensamguk-image@master/icons/1146.jpg`
- 도시 아이콘: `https://cdn.jsdelivr.net/gh/peppone-choi/opensamguk-image@master/game/cast_1.gif`
- 지도 배경: `https://cdn.jsdelivr.net/gh/peppone-choi/opensamguk-image@master/game/map/che/bg_spring.jpg`

## 캐시/버전 전략

- 개발/상시 최신 반영: `@master`
- 릴리스 고정 배포: `@<commit-sha>` 또는 `@<tag>`

운영 환경에서 완전한 재현성이 필요하면 커밋 SHA 고정을 권장합니다.
