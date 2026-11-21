# sunmink4.github.io

직접 만든 앱을 내려받는 GitHub Pages 사이트(Jekyll).

- 앱 하나는 `_projects/<이름>.md` 하나다. 앞머리의 `repository`, `downloads` 로 다운로드 버튼을 만든다.
- 다운로드 버튼과 버전은 브라우저가 GitHub 최신 릴리스를 읽어 채운다 (`assets/js/releases.js`).
- 누적 다운로드 수는 GitHub Actions 가 하루 한 번 `_data/download_stats.json` 에 모은다.

로컬 미리보기: `jekyll serve` 후 http://localhost:4000
