## 6공식테마 
- minima
- jekyll-theme-cayman
- jekyll-theme-midnight
- jekyll-theme-minimal
- jekyll-theme-slate
- jekyll-theme-tactile


- 6테마
  - 6공식테마
  - 6공식테마
  - 6종공식테마
  - 공식테마.6종
  - 6종만 “진짜 GitHub Pages 공식 테마”
  - 아까 6종 넘어가 보였던 건 다른 분류야.

- minima
  - Jekyll 기본 테마
  - 블로그용
  - 가장 안정적
- cayman
  - 프로젝트 소개용
  - README 스타일
- midnight
  - 다크 테마
  - 코드 프로젝트용
- minimal
  - 아주 심플
  - 문서/정리용
- slate
  - README 기반
  - 프로젝트 설명용
- tactile
  - 예전 스타일
  - 거의 안 씀 (레거시 느낌)





## Theme
- minima ⭐ (기본값, 제일 무난)
  - ✅minima
  - ❌jekyll-theme-minima
jekyll-theme-cayman
jekyll-theme-slate
jekyll-theme-midnight
jekyll-theme-minimal
jekyll-theme-modernist
jekyll-theme-tactile
jekyll-theme-hacker
jekyll-theme-leap-day
jekyll-theme-merlot
jekyll-theme-time-machine
jekyll-theme-architect
jekyll-theme-dinky


- [Jekyll.Theme](https://jekyllrb.com/docs/themes/)
- [Jekyll.Theme.MinimalMistake](https://github.com/mmistakes/minimal-mistakes)
- [제킬.테마.검색](http://jekyllthemes.org/)


- 공식테마
  - 테마종류
    - 공식테마
    - 커스텀적
    - 공식 테마는 진짜 소수고, 나머지는 거의 전부 개인·팀이 만든 커스텀 테마라고 보면 됨.
  - Jekyll 자체 공식 테마 ❌ (거의 없음)
  - GitHub Pages가 공식 지원하는 테마 ⭕ ← 우리가 말하는 “공식 테마”


- 확장테마
  - “GitHub Pages 테마”라고 불리는 것들 (확장 개념)



## minimal-mistakes
```bash
remote_theme: mmistakes/minimal-mistakes
plugins:
  - jekyll-remote-theme
  - jekyll-include-cache
minimal_mistakes_skin: dark
```




## ❌Moonwalk
- 테마를 못갖고옴.
- 뭔가충돌되든.
- 어디서가져와야되는데.
- 그걸못함.
- 브라우저문제같기도하고.
- 다크테마를 못가져오는거같음.
- 아...
  - 설마 이게6년전꺼라
  - 못가져오는건가.
  - ㅇㄴ
  - 맞을듯하다.
  - 쎄함이 맞을듯.
  - 다른 파비콘이런것 싹다가져오는데.
  - 흠.
  - 폴더구조문제같기도한데.
- 아...
  - 부트스트랩.
  - 이거일듯.
  - fork하고 뭐 거시기 이게있네.
  - 아...
  - 그래서 Star이것도 
  - 400개대에서 멈춘듯.
  - 무조건적지원ㄴㄴ인듯.
- 버리자ㄱㄱ.
  - 시간아깝다.
  - 더좋은것더많다.
  - 더좋은것더후딱대체ㄱㄱ.




- 4️⃣ index.md 예시 (이거 없으면 빈 화면)
````md
---
layout: home
title: Home
---
# Hello Moonwalk 🌙
This is my site.
````



- Moonwalk는 home 레이아웃이 없음




```bash
title: NangMan
description: Moonwalk test
theme: null

remote_theme: abhinavs/moonwalk

plugins:
  - jekyll-remote-theme
  - jekyll-seo-tag
```
- 현행되는것
- `jekyll-seo-tag`
- 디폴트적.
- 없으면걍싹나가리.



- ❌Moonwalk
  - 현행실패
  - 토큰받으라는거보니
  - 뿌리는것일듯함.


```bash
# Moonwalk remote theme 설정
remote_theme: abhinavs/moonwalk
```
```bash
# Moonwalk remote theme 설정
remote_theme: abhinavs/moonwalk
plugins:
  - jekyll-remote-theme
```



- remote_theme
  - remote_theme: 에 테마의 GitHub repo를 지정하면 된다 
  - 예: abhinavs/moonwalk




- 엣지확인
  - 크롬.라이트
  - 엣지.다크
  - 뭔가좀다르게보나봄.
- 안되는듯.
  - 기본적으로
  - MoonWalk
  - 이쪽에서
  - 더안날라오는듯.


- 다른테마들은
  - 확실히
  - 본인들이요구하는
  - 세팅들이있음.
  - 문제는
  - 이걸안쓰면
  - 싹다나가리가된다는것.
  - 더좋은것일수록
  - 더복잡하다는.
  - 더복잡할수밖에없다는.
  - 어려워지는형태.
  - 난잡해지는형태.
- 커스텀
  - 싹다
  - 개별성이너무강해.
  - 각원하는설정들이
  - 다다른듯.
  - 설정에맞춰줘야진행하고.
  - 그아니면
  - 싹다나가리.
  - MoonWalk이것만보더라도그런듯.
- 결국
  - 설정없이도
  - 싹다다잡아줄수있는.
  - 그런거하는게
  - 실력인듯.
  - 실력일듯.




##
- [ ] chirpy
- theme: jekyll-theme-chirpy
- 이것만으로ㄴㄴ.
- 구조다른거요구하나봄.
- 얘도귀찮.
- 버림ㄱㄱ.


Chirpy 올바른 설치 방법 (이게 정답)
1️⃣ 템플릿 레포 사용 (필수)
👉 이걸로 새 레포 만들어야 함
https://github.com/cotes2020/chirpy-starter




## 반영
- 캐시충돌인듯.