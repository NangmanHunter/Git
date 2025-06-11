# IgnoreGit
##
- [Github▶️GitIgnore(Ko)](https://docs.github.com/ko/get-started/git-basics/ignoring-files)
- [Github▶️GitIgnore(En)](https://docs.github.com/en/get-started/git-basics/ignoring-files)


```bash
touch .gitignore
```
```bash
git rm --cached FILENAME
```
```bash
git rm --cached -r .
```
- .: 현재 디렉토리의 모든 파일과 폴더
- -r: 폴더(디렉토리)도 재귀적으로 처리



## FileIgnore
- ```.gitignore
  📄File
  ```
## DirectoryIgnore
- ```.gitignore
  📁Directory/
  ```
- ```.gitignore
  📁Directory
  ```

## FileTrackDirectoryIgnore
- ```.gitignore
  📁Directory/
  !📁Directory/📄File
  ```
## DirectoryTrackDirectoryIgnore
- ```.gitignore
  📁01Directory/
  !📁01Directory/📁02Directory/
  ```
