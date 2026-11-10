# 러닝 페이스 계산기 (설치형 웹앱)

폴더 안의 파일 6개를 모두 같은 위치에 올리면 됩니다.

- index.html
- manifest.webmanifest
- sw.js
- icon-192.png, icon-512.png, icon-maskable-512.png, apple-touch-icon.png

## 1. 인터넷에 올리기 (무료)

설치형 웹앱은 보안 주소(https)에서만 설치할 수 있어서 호스팅이 필요합니다.

### 방법 A. Netlify Drop (가장 쉬움)
1. 압축을 풀어 폴더를 만듭니다.
2. app.netlify.com/drop 에 접속해 폴더를 화면에 끌어다 놓습니다.
3. 몇 초 뒤 주소(예: https://이름.netlify.app)가 생깁니다.

### 방법 B. GitHub Pages
1. GitHub에서 새 저장소(Public)를 만듭니다.
2. Add file > Upload files 로 파일 6개를 올립니다.
3. Settings > Pages 에서 Branch를 main, 폴더를 / (root)로 저장합니다.
4. 1~2분 뒤 https://아이디.github.io/저장소이름/ 주소가 열립니다.

## 2. 휴대폰에 설치하기

- iPhone: Safari로 주소를 열고 공유 버튼 > "홈 화면에 추가"
- 안드로이드: Chrome으로 주소를 열고 메뉴(⋮) > "앱 설치" 또는 "홈 화면에 추가"

한 번 열어 두면 이후에는 비행기 모드에서도 실행됩니다. 글꼴은 처음 한 번 인터넷으로 받아 저장하고, 받지 못한 상태에서는 기본 글꼴로 표시됩니다.

## 3. 수정해서 다시 올릴 때

sw.js 맨 위의 `const CACHE = 'pace-v1';` 숫자를 pace-v2처럼 올리면, 이미 설치한 앱에도 새 버전이 반영됩니다.

## 4. 내 컴퓨터에서 먼저 확인하기

폴더에서 `python3 -m http.server 8000` 을 실행하고 브라우저에서 http://localhost:8000 을 열면 됩니다.
