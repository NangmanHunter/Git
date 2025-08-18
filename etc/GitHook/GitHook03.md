## 🧠 유명한 사용 사례

| 사용 목적       | 예시                                             |
| ----------- | ---------------------------------------------- |
| ✅ 코드 검사     | ESLint, Prettier, Black 등과 연결                  |
| ✅ 커밋 메시지 규칙 | `commitlint`, Conventional Commit 포맷 강제        |
| ✅ 테스트 자동 실행 | 커밋/푸시 전에 테스트 실행 후 실패 시 중단                      |
| ✅ 보안 검사     | `pre-commit` 훅에서 `truffleHog`, `gitleaks` 등 실행 |

---

## 🚀 유명 툴: **pre-commit 프레임워크**

* Git hook을 **편하게 관리**하게 도와주는 툴
* 다양한 언어의 검사기/툴들을 쉽게 연결 가능
* 설정 한 번 해두면 팀 전체가 같은 검사 환경 사용 가능

```bash
pip install pre-commit

# .pre-commit-config.yaml 작성 후
pre-commit install
```

GitHub 오픈소스 대부분이 `pre-commit` 프레임워크를 써.

🔗 공식사이트: [https://pre-commit.com/](https://pre-commit.com/)
---




## ✅ 요약
* 커밋/푸시/머지 같은 동작에 **자동화된 검사, 테스트, 포맷터** 적용 가능
* Git 자체 기능 + 외부 프레임워크(`pre-commit`) 조합이 강력함

---

궁금하면 `pre-commit`이나 `commit-msg`에서 어떤 포맷 강제를 거는지도 예제로 보여줄 수 있어!
