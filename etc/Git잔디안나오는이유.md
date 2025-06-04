

```bash
git log
```


##
GitHub에서 레포지토리가 **public**인데도 **커밋(push)해도 잔디(기여도 그래프)가 안 칠해지는 이유**는 여러 가지가 있을 수 있습니다. 가장 흔한 원인부터 체크해볼게요.

---

## ✅ 잔디(Contribution Graph)에 안 나오는 주된 이유 5가지

### 1. 🔑 커밋 이메일이 GitHub 계정과 연결되지 않음 ❌

**가장 흔한 이유입니다!**

#### 📌 체크 방법:

* 커밋한 기록에서 커밋 이메일 확인:

  ```bash
  git log
  ```
* 나오는 이메일이 GitHub 계정에 등록되어 있어야 잔디가 채워집니다.

#### ✅ 해결 방법:

1. [https://github.com/settings/emails](https://github.com/settings/emails) 들어가기
2. 커밋에 사용한 이메일이 등록되어 있는지 확인
3. 등록 안 되어 있다면 추가해 주세요

또는 아래 명령어로 이메일 변경:

```bash
git config --global user.email "your-email@example.com"
```

---

### 2. ✅ GitHub 계정 이름과 연결된 사용자가 커밋하지 않음

* 예: A라는 계정으로 push 했는데, 커밋에는 B라는 계정의 이메일이 들어가 있음 → 잔디 안 칠해짐

---

### 3. ✅ 커밋이 `default branch`에 포함되지 않음

* `main`, `master`가 **기본 브랜치**인데,
  다른 브랜치(ex: `dev`, `feature-x`)에만 커밋하면 잔디에 안 나옵니다.

#### ✅ 해결:

* push한 브랜치가 `main`인지 확인하세요.
* 아니면 해당 커밋이 기본 브랜치에 **병합(Merge)** 되어야 잔디에 뜹니다.

---

### 4. ✅ 커밋 날짜/시간이 잘못 설정됨

* 시스템 시간이 잘못되었거나 미래 날짜/예전 날짜로 커밋됨
  → 잔디에 안 보일 수 있음

#### 확인:

```bash
git log --pretty=fuller
```

---

### 5. ✅ force push 후 히스토리가 꼬인 경우

* 기존 커밋이 덮여서 잔디도 날아가는 경우 있음

---

## ✅ 확인 순서 요약

| 확인 항목                     | 확인 방법                                    |
| ------------------------- | ---------------------------------------- |
| 이메일이 GitHub 계정에 등록되어 있는가? | `git config user.email` + GitHub 설정 비교   |
| 커밋한 브랜치가 default인가?       | GitHub 레포지토리 → Settings → Default branch |
| 커밋에 내 이름/이메일이 있는가?        | `git log`로 확인                            |
| 레포가 public인가?             | 주소창에 로그인 안 된 상태에서 접근해보기                  |
| 날짜가 잘못되지 않았는가?            | `git log`로 커밋 시간 확인                      |

---

## 🎯 예시: 내 이메일이 뭔지 확인하려면

```bash
git config user.email
```

그리고 GitHub에 등록된 이메일 목록 확인:
👉 [https://github.com/settings/emails](https://github.com/settings/emails)

---

필요하시면 `git log` 출력 일부를 붙여주시면 더 정확히 진단해드릴게요!
