
##
- PartialCloneIgnore
- PartialDownLoadIgnore
- DownLoadIgnore
- CloneIgnore







## ❌CDN
## 📌 CDN과의 차이
* **CDN (Content Delivery Network)**
  → 말 그대로 “콘텐츠 전달망”이라, 요청할 때마다 **HTTP(S) 요청을 통해 원격에서 불러와 쓰는 것**이에요.
  → 파일을 "내 서버에 저장"하는 게 아니라, 필요할 때마다 원격에서 가져다 씀.
  → 즉 **매번 호출 구조**. (브라우저 캐싱은 가능하지만, 원천적으로 네트워크 호출 기반)

---

## 📌 Git clone처럼 "파일 자체만 부분적으로 받기"
이건 **CDN 개념이 아니고**, Git 저장소 다운로드 관련 개념이에요.

### 방법 1. **Sparse Checkout**

Git은 저장소 전체가 아니라 **일부 디렉토리만 체크아웃**할 수 있습니다.

```bash
git clone --filter=blob:none --no-checkout https://github.com/USER/REPO.git
cd REPO
git sparse-checkout init --cone
git sparse-checkout set path/to/subfolder
```

👉 이렇게 하면 원하는 하위 폴더만 내려받을 수 있어요. (`git clone`의 부분 버전 느낌)

### 방법 2. **git archive**

특정 하위 디렉터리나 파일만 압축으로 뽑아오기 가능.

```bash
git archive --remote=https://github.com/USER/REPO.git HEAD path/to/file > file.zip
```

### 방법 3. **수동 다운로드 (웹 UI)**
GitHub 웹에서 하위 폴더 단위로는 직접 다운로드 불가.
→ 대신 GitHub API나 `DownGit` 같은 툴을 써서 특정 폴더/파일만 zip으로 받을 수 있어요.
---

## 📌 정리
* **CDN** = 원격 파일을 매번 불러다 쓰는 방식 (호출 구조).
* **git clone / sparse-checkout** = 저장소 일부를 **실제 파일로 내려받아 보관**하는 방식.

👉 따라서 말씀하신 건 \*\*CDN이 아니라 "부분 clone"이나 "부분 다운로드"\*\*에 가까워요.



