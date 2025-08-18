## ✅ 해결 방법: hook 파일을 공유하고 싶을 때는?

### 방법 1: 커밋 가능한 디렉토리로 이동 후 `core.hooksPath` 설정하기
1. 예를 들어, 프로젝트 안에 `.githooks/`라는 디렉토리 만든 후:
```
your-project/
├── .githooks/
│   └── pre-commit
```

2. `.githooks/pre-commit` 파일에 원래 쓰던 내용 넣고

3. 실행 권한 부여:

```bash
chmod +x .githooks/pre-commit
```

4. Git에게 그 경로를 사용하라고 설정:

```bash
git config core.hooksPath .githooks
```

> 이제부터 `.git/hooks/` 대신 `.githooks/` 아래 파일을 실행함!

이렇게 하면 Git에 커밋도 되고, 다른 사람도 사용할 수 있어.
협업할 땐 `README`에 설정법 써두면 좋아.








---

### 방법 2: Husky (JavaScript 프로젝트용)

JavaScript 기반 프로젝트라면 [**Husky**](https://typicode.github.io/husky/#/) 같은 툴을 써서 Git hook을 쉽게 공유하고 관리할 수 있어.

---

## 📌 정리

| 질문                        | 답변                                 |
| ------------------------- | ---------------------------------- |
| `.git/hooks/`에 있는 파일 커밋돼? | ❌ 커밋 안 됨 (로컬 전용)                   |
| 공유하려면?                    | ✅ 프로젝트 내부 폴더 + `core.hooksPath` 설정 |
| 다른 사람과 공유 가능?             | ✅ `.githooks/`나 Husky 등으로 가능       |

---
필요하면 `.githooks/` 구조 예시나 설정 스크립트도 만들어줄게!