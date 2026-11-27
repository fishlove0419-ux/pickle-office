# 엘땅고 비서실

이인경 원장님 전용 비서실 — 오피스 맵(클레이 3D·도면) · 회의실 · 작업실 · 비서현황 · AI한도 · 메모.

- 공개 주소: https://fishlove0419-ux.github.io/pickle-office/
- 구성: `index.html` 단일 파일 + `office-clay.png` (외부 라이브러리 없음)
- 저장: 기본은 이 브라우저(localStorage). 헤더의 `로컬 저장` 배지를 눌러 Firebase Realtime Database 주소를 넣으면
  `office/board` · `office/chat` · `office/notes` 경로로 실시간 동기화됩니다.
- 회의실은 `@피쉬`처럼 이름을 지목해 지시를 남길 수 있고, 로컬 모드에서는 확인 답장이 예시로 달립니다.

## Firebase 규칙 예시 (테스트용)

```json
{ "rules": { "office": { ".read": true, ".write": true } } }
```
