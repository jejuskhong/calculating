# 기본 사칙연산 계산기

`index.html` 한 파일로 실행하는 반응형 계산기입니다. 사칙연산, 소수점, 부호 변경, 초기화와 키보드 입력을 지원합니다.

## GitHub Pages

저장소의 **Settings → Pages → Build and deployment**에서 **Deploy from a branch**, **main**, **/(root)**를 선택하고 저장합니다.

예상 주소: https://jejuskhong.github.io/calculating/

위 주소는 Pages 배포가 완료되어야 사용할 수 있습니다.

## Firebase 댓글

기본 댓글 UI와 실시간 조회·등록·본인 댓글 삭제 코드가 포함되어 있습니다. 실제 사용에는 Firebase 프로젝트 연결이 필요합니다. [설정 방법](FIREBASE-SETUP.md)을 참고하세요.

`index.html`의 `firebaseConfig`에 웹 앱 설정값을 입력하고, Firebase에서 익명 로그인을 활성화한 뒤 [firestore.rules](firestore.rules)를 Firestore 규칙에 게시하세요. GitHub에 규칙 파일을 올리는 것만으로 Firebase에 적용되지는 않습니다.

Firebase 웹 앱 설정은 브라우저에 공개되는 값입니다. 서비스 계정 비밀키는 저장소에 올리지 마세요.

## 검증 상태

사칙연산 등 계산 로직 7개 사례와 JavaScript 구문을 확인했습니다. 실제 Firebase 프로젝트 연결, 보안 규칙 배포, 브라우저 간 댓글 공유 및 GitHub Pages 배포는 아직 검증되지 않았습니다.
