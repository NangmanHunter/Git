# GitIgnore
Source
- [Github▶️GitIgnore(Ko)](https://docs.github.com/ko/get-started/git-basics/ignoring-files)
- [Github▶️GitIgnore(En)](https://docs.github.com/en/get-started/git-basics/ignoring-files)


## ExistingFile`GitIgnore`
📄File
```bash
git rm --cached FILENAME
```


📄AllFile
```bash
git rm --cached -r .
```
- .: 현재 디렉토리의 모든 파일과 폴더
- -r: 폴더(디렉토리)도 재귀적으로 처리
- VsCode에서 바로반영안될때있음.
  - 실제로는 반영되었어도 화면상으로는 잡히는경우있음.
  - VsCode재실행ㄱㄱ.



## FileTrackDirectory`GitIgnore`
- ```.gitignore
  📁Directory/
  !📁Directory/📄File
  ```


## DirectoryTrackDirectory`GitIgnore`
- ```.gitignore
  📁01Directory/
  !📁01Directory/📁02Directory/
  ```
