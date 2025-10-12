## 현행최적
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git

git sparse-checkout init
git sparse-checkout set src/GitIgnore
git checkout HEAD

Remove-Item src/*.*
Remove-Item ./*.*
```
- 되긴하는데.
- 너무번거롭다.
- 현행비최적.
- 좀더최적화-더필요한듯.
- 혹은-아싸리다른대안-더ㄱㄱ.



##
- `clone`
- `sparse-checkout`
- `.git`삭제


```
clone
sparse-checkout
```
.git삭제


##
```
git clone --filter=blob:none --no-checkout
└── .git/          ← 전체 히스토리 저장
└── (워킹 디렉토리 없음)

git sparse-checkout set path/to/subfolder
└── path/to/subfolder/  ← 선택한 폴더만 실제 파일 다운로드
```






##
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git
```
```
git sparse-checkout init --cone
```
```
git sparse-checkout set src/GitIgnore
```


## 하위까지다받기
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git
```
```
# sparse-checkout 초기화
git sparse-checkout init

# 필요한 파일/폴더 지정
git sparse-checkout set src/GitIgnore

# HEAD 체크아웃
git checkout HEAD
```
- 헤드부터
- 하위까지
- 받아짐.


```
📁src
- 📁GitIgnore
  - 📄
- 📄
```
- src-✅GitIgnore폴더ㆍ✅src파일ㆍ❌src하위폴더
- GitIgnore폴더-GitIgnore파일


❌
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git
```
```
# 1. sparse-checkout 초기화 (non-cone)
git sparse-checkout init

# 2. 원하는 폴더 내부 파일만 선택
git sparse-checkout set src/GitIgnore/.gitignore src/GitIgnore/test.md

# 3. 체크아웃
git checkout HEAD
```
- Git하위파일-src하위파일도 받아짐.


❌
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git
```
```
git sparse-checkout init
git sparse-checkout set "src/GitIgnore/*"
git checkout HEAD
```
- 안받아짐.


## 받고삭제
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git
```
```
git sparse-checkout init
git sparse-checkout set src/GitIgnore
git checkout HEAD

# 상위 폴더에 있는 원치 않는 파일 삭제
Remove-Item src/*.md
```
- 다받고
- src파일삭제형.


## src하위모든파일
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git
```
```
git sparse-checkout init
git sparse-checkout set src/GitIgnore
git checkout HEAD

Remove-Item src/*.*
```
- 모든파일


## Git하위모든파일
```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git
```
```
git sparse-checkout init
git sparse-checkout set src/GitIgnore
git checkout HEAD

Remove-Item src/*.*
Remove-Item ./*.*
```
- `./`-예약어
- `.`-예약어
- `.`👉❌폴더
- `.`👉❌폴더-애당초못만들게만들어놓음-예약어로잡혀있게.
- `.`👉❌폴더만들지말것.
- `.A`👉✅폴더
- `.A`👉✅폴더-이건가능




```
git clone --filter=blob:none --no-checkout https://github.com/NangmanHunter/Git.git
cd Git

git sparse-checkout init
git sparse-checkout set src/GitIgnore
git checkout HEAD

Remove-Item src/*.*
Remove-Item ./*.*
```




## 경로확인
바로자식
git ls-tree -d HEAD


전체자식
git ls-tree -r --name-only HEAD


폴더전체자식
git ls-tree -r --name-only HEAD | Select-String "src/GitIgnore"




##
글고보니.
- 아싸리
세팅되는것들
그냥싹다
한데
.git에다모아놓고.
- 그다음 받아서
진행하는식.
- 나아가
.git만
지우는식으로.
이것도
상당좋을듯.ㄱㄱ.


