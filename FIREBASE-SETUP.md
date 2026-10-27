# Firebase 댓글 연결

1. Firebase 콘솔에서 웹 앱을 등록하고 프로젝트 설정의 `firebaseConfig` 값을 `index.html`의 같은 이름 객체에 넣습니다. 서비스 계정 키는 사용하지 않습니다.
2. Authentication → 로그인 방법에서 **익명**을 사용 설정합니다.
3. Cloud Firestore 기본 데이터베이스를 만들고 규칙 탭에 `firestore.rules` 내용을 붙여 넣어 게시합니다.
4. `index.html`을 HTTP/HTTPS 웹 서버에서 열어 댓글 등록과 다른 브라우저에서의 조회를 확인합니다.

댓글은 최신 50개를 표시합니다. 같은 익명 로그인 세션에서 작성한 댓글에 삭제 버튼이 나타납니다. 브라우저 데이터를 지우면 작성자 권한을 잃을 수 있습니다.

실제 Firebase 프로젝트 설정이 아직 없어 연결, 규칙 배포 및 서버 저장 검증은 완료되지 않았습니다.

참고: https://firebase.google.com/docs/auth/web/anonymous-auth
https://firebase.google.com/docs/firestore/manage-data/add-data
