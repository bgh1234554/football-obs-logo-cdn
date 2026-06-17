# football-obs-logo-cdn

OBS 축구 오버레이/대시보드 프로젝트(`logos.csv`, `leagues.csv`)에서 쓰는 팀/리그 로고를 GitHub Pages로 호스팅하는 저장소.

## 폴더 구조

```
nt/             국가대표팀 (FA) 로고 - 평면 구조
clubs/<Country>/  클럽 로고 - 국가별 하위 폴더
leagues/        리그/대회 로고 - 평면 구조
```

## 신규 로고 업로드 시 파일명 규칙

- 공백/언더스코어 없는 CamelCase
- 국가대표팀 로고는 `<Country>FA.ext` 형식 (예: `NorwayFA.png`, `BeninFA.svg`)
- 클럽/리그 로고는 ID, 접두사 없이 이름만 (예: `DynamoMoscow.png`, `PremierLeague.png`)

## 사용 예시 (GitHub Pages)

```
https://<username>.github.io/football-obs-logo-cdn/nt/NorwayFA.png
https://<username>.github.io/football-obs-logo-cdn/clubs/Russia/DynamoMoscow.png
https://<username>.github.io/football-obs-logo-cdn/leagues/PremierLeague.png
```

## Issue로 요청할 것

- 새 리그/대회 추가가 필요할 때
- 로고가 옛날 버전(구 엠블럼)이거나 깨져 있을 때
- 위 두 가지를 발견하면 Issue로 남겨서 기록할 것
