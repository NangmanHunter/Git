

- GitHook
- GithubActions

- GitHook >> GithubActions
- 로컬정렬 >> 원격정렬
- 로컬정렬ㆍ원격정렬 >> 원격정렬

## GitHook
Python-blackFommater
- touch .git/hooks/pre-commit
- #!/bin/bash
  echo "📦 Running black formatter..."  
  black .
- chmod +x .git/hooks/pre-commit  





## Path

/bin/bash
- ```bash
  /bin/bash
  ```
- ```bash
  \bin\bash
  ```
- ```bash
  C:\Program Files\Git\bin\bash
  ```

/
- ```bash
  /
  ```
- ```bash
  \
  ```
- ```bash
  C:\Program Files\Git\
  ```


## Powershell
- Powershell
  - powershell -ExecutionPolicy Bypass -File .\myscript.ps1
  - powershell -ExecutionPolicy Bypass -File .\SortedbyLineDirectory05.ps1
- Git Bash
  - powershell.exe -ExecutionPolicy Bypass -File ./myscript.ps1
  - powershell.exe -ExecutionPolicy Bypass -File ./SortedbyLineDirectory05.ps1
  - powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/test/etc/SortedbyLineDirectory05.ps1

pre-commit
- #!/bin/bash
  echo "📦 Running SortLineDirectory formatter..."  
  powershell.exe -ExecutionPolicy Bypass -File ./etc/SortedbyLineDirectory05.ps1
  powershell.exe -ExecutionPolicy Bypass -File ./etc/SortedbyLineDirectory05.ps1
  powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/test/etc/SortedbyLineDirectory05.ps1
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectory formatter..."  
  powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/test/etc/SortedbyLineDirectory05.ps1
  ```


❌\
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"  
  powershell.exe -ExecutionPolicy Bypass -File C:\github-nangmanhunter\test\.git\hooks\SortLineDirectoryResure.ps1
  ```
✅\\
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"  
  powershell.exe -ExecutionPolicy Bypass -File C:\\github-nangmanhunter\\test\\.git\\hooks\\SortLineDirectoryResure.ps1
  ```
✅/  
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"
  powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/test/.git/hooks/SortLineDirectoryResure.ps1
  ```
✅"/"  
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"
  powershell.exe -ExecutionPolicy Bypass -File "C:/github-nangmanhunter/test/.git/hooks/SortLineDirectoryResure.ps1"
  ```  
✅"\\"  
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"
  powershell.exe -ExecutionPolicy Bypass -File "C:\\github-nangmanhunter\\test\\.git\\hooks\\SortLineDirectoryResure.ps1"
  ```  

✅"\"
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"  
  powershell.exe -ExecutionPolicy Bypass -File "C:\github-nangmanhunter\test\.git\hooks\SortLineDirectoryResure.ps1"
  ```
  - 경로복사
  - Shift+Alt+C
  - "" + 붙여넣기

❌"    "
- ```bash
      #!/bin/bash
      echo "📦 Running SortLineDirectoryRecurse"  
      powershell.exe -ExecutionPolicy Bypass -File C:\\github-nangmanhunter\\test\\.git\\hooks\\SortLineDirectoryResure.ps1
  ```



## ✅권한부여

```bash
chmod +x .git/hooks/pre-commit
```
- ❌PowerShell
- ✅GitBash
ㄴ이것해줘야됨



- 파일작성👉권한부여👉Commit

Hook
- 파일작성
- 권한부여



## 파일작성
- echo "echo '🛠️ pre-commit hook running...'" > .git/hooks/pre-commit  
- echo "echo '🛠️ pre-commit 
hook running...'" > .git/hooks/pre-commit  
- cat << 'EOF' > .git/hooks/pre-commit
#!/bin/bash
echo "📦 Running black formatter..."
black .
EOF

- printf '#!/bin/bash\nblack .\necho "✅ Done formatting"\n' > .git/hooks/pre-commit
- printf '#!/bin/bash
black .\necho "✅ Done formatting"\n' > .git/hooks/pre-commit
- printf '#!/bin/bash
black .
echo "✅ Done formatting"\n' > .git/hooks/pre-commit
- printf '#!/bin/bash
black .
echo "✅ Done formatting"' > .git/hooks/pre-commit

- printf '#!/bin/bash
black .
echo "✅ Done formatting"' > .git/hooks/pre-commit


파일작성
- printf '#!/bin/bash
  echo "📦 Running SortLineDirectory formatter..."  
  powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/test/etc/SortedbyLineDirectory05.ps1

- printf '#!/bin/bash
echo "📦 Running SortLineDirectory formatter..."  
powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/test/etc/SortedbyLineDirectory05.ps1



- ⭕ 
cat << 'EOF' > .git/hooks/pre-commit
#!/bin/bash
echo "📦 Running SortLineDirectory formatter..."  
powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/test/etc/SortedbyLineDirectory05.ps1
EOF  
ㄴ경로주의.!!!
ㄴpowershell -> \
ㄴgit-bash   -> /

- ❌
cat << 'EOF' > .git/hooks/pre-commit
#!/bin/bash
echo "📦 Running SortLineDirectory formatter..."  
powershell.exe -ExecutionPolicy Bypass -File C:\github-nangmanhunter\test\etc\SortedbyLineDirectory05.ps1
EOF  
ㄴ경로바꿔줘야함.!!!
ㄴ아...
ㄴ짜증나네.
ㄴ그렇다면
ㄴ아싸리.
ㄴ경로받아다가
ㄴ바꿔서
ㄴ변수로
ㄴ넣는식으로ㄱㄱ.!!!



##
cat
- concatenate
<<
- here document
<< 'EOF'
- EOF라는 키워드가 나올 때까지


cat << 'EOF' > .git/hooks/pre-commit
(여기에 쓸 내용들)
EOF





##
- Git Bash
- touch .git/hooks/pre-commit
- cat << 'EOF' > .git/hooks/pre-commit
#!/bin/bash
echo "📦 Running black formatter..."
black .
EOF
- chmod +x .git/hooks/pre-commit


```bash
touch .git/hooks/pre-commit

cat << 'EOF' > .git/hooks/pre-commit
#!/bin/bash
echo "📦 Running SortLineDirectory formatter..."  
powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/quote/etc/AutoScript/Sort.ps1
EOF

chmod +x .git/hooks/pre-commit
```


```bash
touch .git/hooks/pre-commit

cat << 'EOF' > .git/hooks/pre-commit
#!/bin/bash
echo "📦 Running SortLineDirectory formatter..."  
powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/quote/etc/AutoScript/Sort.ps1
EOF
```


```bash
touch .git/hooks/pre-commit

cat << 'EOF' > .git/hooks/pre-commit
#!/bin/bash
echo "📦Sort"  
powershell.exe -ExecutionPolicy Bypass -File C:/github-nangmanhunter/quote/etc/AutoScript/Sort.ps1

echo "🎁Add" 
git add .

echo "Sort▶️Add▶️Commit" 
EOF
```
ㄴ혹여나
ㄴ나중에안되면.
ㄴchmod
ㄴ추가ㄱㄱ.



## ❌\
Linux
- ✅/
- ❌\

window
- ✅/
- ✅\


##
ls -l .git/hooks/pre-commit
- -rwxr-xr-x ▶️ 권한있음
- -rw-r--r-- ▶️ 권한없음

ls -l .git/hooks
- -rwxr-xr-x

##
-rwxr-xr-x 1 nangman-hunter 197121 3650  1월 25 00:28 update.sample*

1
하드 링크 수
원본보호위해-링크개념도입->하드.링크.
->다양한 접근경로를 제공하기위한방식



## 이모지깨짐
Encoding
- locale
- UFT-8

Font
ㄴGitBash에서
ㄴ폰트다르게설정해도
ㄴ안먹음.
ㄴ애당초
ㄴ애물레이터.
ㄴ얘가.
MinTTY기반이라는데.
ㄴ여기서
ㄴ폰트제한되나봄.!!!
그래서
ㄴpowershell은되나.
ㄴgitbash는안됨.!!!
ㄴ이게
ㄴ계속이상했던것.!!!
😘 -> ❌
▶️ -> ⭕
ㄴgitbash에서
ㄴ지원하다말음.!!!


GitBash
- ❌ Font


방법.
ㄴ우회.!!!
ㄴpowershell에서
ㄴGitBash사용.!!!
ㄴ사실.
ㄴWSL로되버림.!!!
ㄴ엄밀한
ㄴGitBash아닌.
그럼에도
ㄴLinux형태라.
ㄴ아싸리
ㄴGitBash와
ㄴ너무도동지형태로
ㄴ싹다
ㄴ명령어호환됨.!!!
ㄴ이게
ㄴ너무좋음.
ㄴ너무강력함.!!!
ㄴㄱㄱ.!!!
글고보니
ㄴWSL
ㄴ여긴또
ㄴ지원되네?!

결국
ㄴGitBash만
ㄴ안되는상황.
ㄴ걍
ㄴ폰트미지원이라
ㄴ그런가봄.
ㄴㅇㄴ.

powershell-bash -> WSL -> GitBash
ㄴ우선순위로작용.
ㄴ그렇기에
ㄴWSL켜짐.!!!

결국
ㄴ폰트.


- ⭕ PowerShell
- ⭕ WSL
- ❌ GitBash

그렇기에
ㄴ우회.
ㄴㄱㄱ.

PowerShell -> ⭕WSL
PowerShell -> ❌GitBash


PowerShell -> bash -> WSL



## GitHook종류
- pre-commit      ▶️커밋 직전에 실행됨. 코드 포맷 검사, 테스트 실행 등
- commit-msg      ▶️커밋 메시지를 작성한 후, 커밋 확정 전 실행됨. 메시지 형식 검사 등에 사용
- pre-push        ▶️git push` 하기 직전에 실행. 테스트 실패 시 푸시 막기 가능
- pre-merge-commit▶️병합 직전에 실행                            
- post-commit     ▶️커밋이 완료된 후 실행                         
- post-merge      ▶️병합이 끝난 뒤 실행


택일
- ✅pre-commit


## ❌.sample
```
.git/hooks/
├── pre-commit.sample
├── commit-msg.sample
└── pre-push.sample
```
- .git/hooks/
- .sample` 확장자
- .sample지우고수정하면 실제동작


## ❌GitHub
GitHub
- ❌.git/hooks/
- ✅.githooks/

.git/hooks/ 디렉토리는 Git 저장소 내부의 설정 디렉토리(.git)에 포함된 로컬 전용 설정 영역
* 이 디렉토리는 **Git이 자동으로 생성**하는 것
* Git은 `.git/` 폴더 자체를 **버전 관리 대상에서 제외**함
그래서 그 안의 파일들인 `pre-commit`, `post-commit` 등도 커밋되지 않아.

.git/hooks/ 대신 .githooks/ 아래 파일을 실행

`.git/hooks/` 안에 있는 hook 스크립트들은 기본적으로 Git에 커밋되지 않아


## 출력위치
- ✅출력
- ❌터미널


터미널 vs 출력
- 터미널: 일반적으로 사용자가 직접 명령어를 실행한 결과가 출력됨.
- 출력: Visual Studio Code 같은 에디터에서 확장 기능, Git, 훅 등 내부 프로세스가 실행한 로그가 나옴.

왜 pre-commit 훅의 결과가 터미널이 아닌 출력에 표시될까?
- pre-commit 훅은 Git 내부에서 백그라운드 프로세스처럼 실행됨.
- 특히 VS Code 같은 GUI 환경에서는 Git 명령이 터미널을 거치지 않고 직접 실행돼.
- 이때 Write-Host나 echo 등의 출력은 출력 창으로 리디렉션됨.
- → 그래서 너는 VS Code 안에서 Git 커밋을 할 때 Write-Host 메시지가 터미널이 아니라 출력에 뜨는 거야.


## .git보기
❌ls
- ```bash
  ls
  ```

Linux
- ```bash
  ls -a
  ```
- ```bash
  ls -al
  ```
  - -a → 숨김 포함
  - -l → 자세히(long) 보기
  - ✅Linux
  - ❌PowerShell

PowerShell
- ```ps1
  ls -Force
  ```
- ```ps1
  Get-ChildItem -Force
  ```

##
- ```ps1
  ls -Force
  ```
- ```ps1
  cd .git
  ```
- ```ps1
  cd hooks
  ```
- ```ps1
  Out-File "pre-commit"
  ```
- ```ps1
  code pre-commit
  ```
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"  
  powershell.exe -ExecutionPolicy Bypass -File " 📄\..."
  git add .
  ```
- ```bash
  #!/bin/bash
  echo "📦 Running SortLineDirectoryRecurse"  
  powershell.exe -ExecutionPolicy Bypass -File "C:\github-nangmanhunter\Powershell\src\SortLineDirectoryRecurse.ps1"
  git add .
  ```



## ❌CRLF
- ✅LF
- ❌CRLF

Windows에서는 기본이 CRLF인데, Git은 LF만 허용함.
pre-commit 파일 열기
우측 아래에 CRLF → 눌러서 LF로 변경
저장 (Ctrl + S)


## ❌UTF-8 with BOM
- ❌UTF-8 with BOM
- ✅UTF-8
하단
ㄴ클릭
ㄴ인코딩하여저장
ㄴUTF-8
ㄴ저장


##
- 터미널종료
  - ❌파일인식
  - 재실행요함
- Ctrl+`
- GitBash  
- ```bash
  chmod +x .git/hooks/pre-commit
  ```

권한은
ㄴ필요없을듯한데.


확실한건.
ㄴ세팅문제.
ㄴ호환문제.
ㄴ언어문제.
✅UTF-8
- ❌UTF-8 with BOM
✅LF
- ❌CRLF