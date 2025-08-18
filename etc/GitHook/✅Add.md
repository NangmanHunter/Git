## ✅add .
```
...
git add .
```
❌add.
- staging상태≠파일상태
- staging상태≠정렬파일상태
- staging상태≠정렬파일상태👉변경사항새로발생
- staging상태≠정렬파일상태👉변경사항+
- staging상태≠정렬파일상태👉+변경사항
- 계속반복

대응
- addx2
  - 누적성
  - 중첩성
  - 안전성
  - 중첩성>>편의성
  - 안전성>>편의성
- add이전단계.
  - 편의성
  - ❌안전성



✅add.
- staging상태
- staging상태👉정렬파일
- staging상태👉정렬파일👉Staging추가
- staging상태👉정렬파일👉Staging추가👉staging상태=파일상태👉❌변경사항

결국
- ❌Staging👉정렬👉Commit
- ❌Staging👉정렬👉Commit👉✅Stagingㆍ❌정렬
- ✅Staging👉정렬👉Staging👉Commit
- ✅Staging👉정렬👉Staging👉Commit👉✅Stagingㆍ✅정렬
- ✅Staging👉정렬👉add👉Commit
- ✅add👉정렬👉add👉Commit


즉
- Staging
- 정렬
- Commit
  - ✅StagingCommit
  - ❌정렬Commit
- ❌정렬Staging
- 변경사항잔존


##
파일구조
❌
```
- Script
```
- ```
  - Script
  ```
- ```
  - Log
  - Script
  ```

✅
```
- Script
- add
```
- ```
  - Script
  - add
  ```
- ```
  - Log
  - Script
  - add
  ```

## ✅add필수
pre-commit 훅에서 파일을 수정한다면, git add는 사실상 필수


내용변경
ㄴ✅add .
ㄴ필수
ㄴScript
ㄴpre-commit + add

단순로그
ㄴ❌add .
ㄴLog
ㄴpre-commit


