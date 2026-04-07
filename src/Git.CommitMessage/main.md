## CommitMessage
- [x] `feat`
- [x] `fix`
- [x] `docs`


## GitCommitMessage
Form
```bash
<type>(<scope>): <subject>

<body>

<footer>
```
```bash
feat(ui): add responsive layout for mobile
fix(auth): correct token validation logic
docs: update contribution guide
refactor: simplify database query structure
```


## Type
| type         | 의미                    | 예시                                      |
| ------------ | --------------------- | --------------------------------------- |
| **feat**     | 새로운 기능 추가             | `feat: add dark mode`                   |
| **fix**      | 버그 수정                 | `fix: incorrect path handling`          |
| **docs**     | 문서 관련 변경              | `docs: update API usage examples`       |
| **style**    | 코드 포맷, 세미콜론 등 비기능적 수정 | `style: format code with prettier`      |
| **refactor** | 기능 변화 없는 코드 개선        | `refactor: simplify login logic`        |
| **test**     | 테스트 추가/수정             | `test: add unit tests for user service` |
| **chore**    | 빌드, 의존성 등 잡무          | `chore: update dependencies`            |
| **perf**     | 성능 개선                 | `perf: improve image loading speed`     |
| **build**    | 빌드 시스템 변경             | `build: migrate to Vite`                |
| **ci**       | CI/CD 관련 변경           | `ci: add GitHub Actions workflow`       |
| **revert**   | 이전 커밋 되돌리기            | `revert: revert previous change`        |
