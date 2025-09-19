

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
