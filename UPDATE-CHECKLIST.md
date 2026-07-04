# MOA Bodychart 업데이트 체크리스트

새 버전을 GitHub에 올릴 때:

1. `index.html`에서 `const APP_VERSION = "..."` 변경
2. `version.json`의 `version` 변경
3. `version.json`의 `releasedAt`, `title`, `changes` 수정
4. 수정 파일 전체를 GitHub에 업로드
5. 기존 웹앱에서 `더보기 → 업데이트 확인` 테스트
6. 업데이트 배너에서 `백업` 후 `업데이트` 테스트

예시:

- 현재: `1.0.0`
- 다음: `1.0.1`

서비스 워커 로직 자체를 크게 바꿨을 때만 `sw.js`의 `CACHE_NAME`도 `v2`, `v3`처럼 올리면 됩니다.
