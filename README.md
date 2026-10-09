# football-obs-logo-cdn

[OBS Football Dashboard](https://github.com/bgh1234554/football-obs-frontend)에서 쓰는 팀·국가대표 협회·리그 로고를 GitHub Pages로 제공하는 저장소입니다.

API-Football이 주는 로고가 없거나 오래됐거나 화질이 낮을 때 이 저장소의 로고로 대신 보여 줍니다. 대시보드 사용법은 [프런트엔드 저장소](https://github.com/bgh1234554/football-obs-frontend)를 참고하세요.

## 로고가 이상할 때

로고가 옛날 엠블럼이거나 깨져 보이거나, 새 리그·대회 로고가 필요하면 [Issues](https://github.com/bgh1234554/football-obs-logo-cdn/issues)에 남겨 주세요. 팀 이름, 대회, 경기 ID, 화면 캡처를 함께 적어 주시면 확인이 빠릅니다.

## 폴더 구조

```text
clubs/<Country>/   클럽 로고 (국가별 폴더)
nt/                국가대표팀 협회 로고
leagues/           리그·대회 로고
```

## 로고 주소

GitHub Pages 주소 뒤에 파일 경로를 붙입니다.

```text
https://bgh1234554.github.io/football-obs-logo-cdn/<경로>
```

예시:

```text
https://bgh1234554.github.io/football-obs-logo-cdn/leagues/PremierLeague.png
https://bgh1234554.github.io/football-obs-logo-cdn/nt/NorwayFA.png
https://bgh1234554.github.io/football-obs-logo-cdn/clubs/Italy/Juventus.png
```

## 로고 추가하기

1. 아래 규칙에 맞는 이름으로 파일을 해당 폴더에 넣고 `main` 브랜치에 커밋합니다.
2. GitHub Pages가 자동으로 다시 배포합니다. 저장소의 **Actions** 또는 **Deployments**에서 완료를 확인하고, 브라우저에서 로고 주소가 열리는지 확인합니다.
3. 대시보드에 반영하려면 [football-obs-backend](https://github.com/bgh1234554/football-obs-backend)의 CSV에 주소를 등록하고 백엔드를 다시 배포합니다.
   - 팀 로고, 국가대표 협회 로고: `logos.csv`
   - 리그 로고: `leagues.csv`

이 저장소에 파일을 올리는 것만으로는 대시보드에 표시되지 않습니다. 3단계가 필요합니다.

이미 등록된 로고 파일을 같은 이름으로 바꾸면 브라우저 캐시 때문에 바로 반영되지 않을 수 있습니다.

## Issue로 요청할 것

- 새 리그/대회 추가가 필요할 때
- 로고가 옛날 버전(구 엠블럼)이거나 깨져 있을 때

### 파일 이름 규칙

- 공백이나 밑줄 없이 단어 첫 글자를 대문자로 씁니다(CamelCase). 예: `DynamoMoscow.png`
- 클럽과 리그 로고는 ID나 접두사 없이 이름만 씁니다. 예: `PremierLeague.png`
- 국가대표 협회 로고는 `<국가>FA.<확장자>` 형식입니다. 예: `NorwayFA.png`, `BeninFA.svg`

## 권리 안내

로고의 상표권과 저작권은 각 구단, 협회, 대회 주최 측에 있습니다. 이 저장소는 대시보드에 로고를 표시하기 위한 용도이며, 로고 사용 권리를 부여하지 않습니다.

권리자가 삭제나 수정을 요청하면 [Issues](https://github.com/bgh1234554/football-obs-logo-cdn/issues) 또는 [이메일](mailto:bgh1234554@gmail.com)로 연락해 주세요.
