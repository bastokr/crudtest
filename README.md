# crudtest

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

권환 관련 에러 적용 (Cloud Firestore) / 규칙 을 아래와같이 수정 )
service cloud.firestore {
  match /databases/{database}/documents {
    match /{document=**} {
      allow read, write: if request.auth.uid != null;
    }
  }
}


git .참조 사이트 
https://webnautes.tistory.com/1422



git branch -M ㅡmaster


git remote add origin https://github.com/bastokr/crudtest.git