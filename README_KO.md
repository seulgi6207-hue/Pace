# PACE RUN — 아이폰 설치용 웹앱

## 포함 파일
- `index.html`: 러닝 페이스 계산기
- `manifest.webmanifest`: 홈 화면 설치 설정
- `sw.js`: 오프라인 캐시
- `icon.svg`, `icon-192.png`, `icon-512.png`: 앱 아이콘

## 아이폰 설치 방법
1. 아래 배포 방법 중 하나로 폴더 전체를 HTTPS 주소에 올립니다.
2. 아이폰 Safari에서 배포된 주소를 엽니다.
3. 하단(또는 상단) 공유 버튼을 누릅니다.
4. `홈 화면에 추가`를 선택하고 이름이 PACE RUN인지 확인한 뒤 추가합니다.
5. 홈 화면의 PACE RUN 아이콘으로 실행합니다.

## 가장 쉬운 무료 배포: Netlify Drop
1. PC 또는 아이패드에서 https://app.netlify.com/drop 를 엽니다.
2. 압축을 푼 `pace_run_pwa` 폴더를 업로드합니다.
3. 생성된 `https://...netlify.app` 주소를 아이폰 Safari에서 엽니다.
4. 위 설치 방법대로 홈 화면에 추가합니다.

Netlify 계정 로그인/가입이 요구될 수 있으며, 배포 서비스의 정책과 무료 제공 조건은 변경될 수 있습니다.

## GitHub Pages 대안
1. GitHub에 새 저장소를 만듭니다.
2. 이 폴더 안의 파일을 저장소 최상위에 업로드합니다.
3. 저장소 Settings → Pages → Deploy from a branch → `main` / `/(root)`를 선택합니다.
4. 생성된 HTTPS 페이지 주소를 Safari에서 열어 설치합니다.

## 참고
- 이 앱은 서버나 회원가입 없이 동작하는 정적 웹앱입니다.
- 계산은 기기 안에서 수행됩니다. 입력한 기록을 외부 서버로 전송하거나 계정에 저장하지 않습니다.
- PWA 설치와 오프라인 실행을 위해 HTTPS 주소에서 최초 1회 접속해야 합니다.
- iOS 버전 및 Safari 설정에 따라 메뉴 이름이나 설치 동작이 조금 다를 수 있습니다.
