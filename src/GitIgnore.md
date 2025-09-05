# GitIgnore



Source
- [Github▶️GitIgnore(Ko)](https://docs.github.com/ko/get-started/git-basics/ignoring-files)
- [Github▶️GitIgnore(En)](https://docs.github.com/en/get-started/git-basics/ignoring-files)


## Create`GitIgnore`
LinuxShell
```bash
touch .gitignore
```


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


## File`GitIgnore`
```.gitignore
📄File
```

PdfFile`GitIgnore`
```gitignore
*.pdf
```


## Directory`GitIgnore`
- ```.gitignore
  📁Directory/
  ```
- ```.gitignore
  📁Directory
  ```


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
