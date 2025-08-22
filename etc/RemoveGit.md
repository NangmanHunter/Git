
##
```bash
# .git 폴더 통째로 삭제 (히스토리 전부 사라짐)
rm -rf .git  

# 새로 Git 초기화
git init

# 원격 저장소 다시 연결
git remote add origin <원격_저장소_URL>

# 현재 상태를 새로운 최초 커밋으로 추가
git add .
git commit -m "Initial commit (reset history)"

# 원격에 덮어쓰기 (주의: 기존 히스토리 다 날아감)
git push -f origin main

```


