# RemoveGit


## GUI`RemoveGit`
✅Git폴더
- `.git` + Click
- Delete

❌부모폴더
- 부모폴더 + Click
- Delete


## CLI`RemoveGit`
```bash
rm -rf .git
```
<details open>
    <summary></summary>

```bash
rm -rf .git
```
```ps1
Remove-Item -Recurse -Force .git
```
```ps1
if (Test-Path .git) {
    Remove-Item -Recurse -Force .git
    Write-Host ".git 폴더가 삭제되었습니다."
} else {
    Write-Host ".git 폴더가 존재하지 않습니다."
}
```
</details>


##
```bash
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


