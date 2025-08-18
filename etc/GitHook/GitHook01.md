
## GPT

오~ 아주 좋은 질문이야.  
**GitHub에 파일 올릴 때 자동으로 포맷팅(정렬) 스크립트 실행**하고 싶다면,  
→ **가능해!** 다만 GitHub 자체에서는 직접 실행은 안 되고, **로컬이나 CI 도구에서 자동화**하는 방식이야.

---

## 방법 1: **로컬 Git hook (`pre-commit`) 사용**
Git은 커밋 전에 자동으로 실행할 수 있는 **hook**을 지원해.
- `.git/hooks/pre-commit`에 스크립트를 넣으면,
- `git commit` 하기 전에 자동 실행됨.

### 예: Python 포맷팅 자동화
```bash
#!/bin/bash
black .
```

### 사용 방법
1. `.git/hooks/pre-commit` 파일 생성
2. 위 스크립트 내용 저장
3. `chmod +x .git/hooks/pre-commit` 로 실행 권한 부여

> 이러면 커밋 전에 알아서 포맷팅하고 커밋함

---

## 방법 2: **GitHub Actions (CI/CD 자동화)**
파일 푸시(push)될 때 GitHub 서버에서 스크립트를 실행하게 만들 수도 있어.

예: `.github/workflows/format-check.yml`
```yaml
name: Auto Format

on: [push]

jobs:
  format:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Run Formatter
        run: |
          npm install
          npm run format
      - name: Commit changes
        run: |
          git config user.name "github-actions"
          git config user.email "actions@github.com"
          git add .
          git commit -m "Auto format"
          git push
```

단점:
- GitHub 서버에서 포맷 후 다시 **자동 커밋**하므로, **PR에 반영됨**
- 약간 느릴 수 있음

---

## 보너스: **Prettier, ESLint, Black, etc. 자동 적용**
- JavaScript → Prettier + ESLint
- Python → Black + isort
- HTML/CSS → Prettier

---

### 정리
| 방법              | 타이밍           | 특징                          |
|-------------------|------------------|-------------------------------|
| Git Hook          | 커밋 전에        | 로컬에서 자동 포맷            |
| GitHub Actions    | 푸시 후          | 서버에서 포맷 & 자동 커밋 가능 |

---

어떤 언어나 프로젝트인지 말해주면, 거기에 맞춰 **예시 코드** 바로 짜줄 수 있어!



