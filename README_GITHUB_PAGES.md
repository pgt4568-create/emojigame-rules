# 이모지 퀴즈 웹앱 GitHub Pages 배포 파일

이 폴더를 GitHub 저장소에 그대로 업로드하면 됩니다.

## 포함 파일

- index.html: 실제 웹앱 파일
- .nojekyll: GitHub Pages가 Jekyll 처리를 하지 않도록 하는 빈 파일

## 배포 전 필수 작업

index.html을 열고 아래 firebaseConfig 부분을 본인 Firebase 프로젝트 값으로 바꾸세요.

```js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.firebasestorage.app",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

## GitHub Pages 배포 요약

1. GitHub에서 새 public repository를 만듭니다.
2. 이 폴더 안의 index.html, .nojekyll을 업로드합니다.
3. Settings → Pages로 이동합니다.
4. Source: Deploy from a branch
5. Branch: main, Folder: /root
6. Save를 누릅니다.
7. 잠시 후 Actions 또는 Pages 화면에서 배포 주소를 확인합니다.

예상 주소 형태:
https://깃허브아이디.github.io/저장소이름/

## 수업 전 확인

- 학생 기기에서 학생 모드로 제출 테스트
- 선생님 기기에서 선생님 모드로 제출 목록 실시간 확인
- 정답 공개 버튼 작동 확인
- 수업 후 Firestore 규칙 잠그기 또는 데이터 삭제
