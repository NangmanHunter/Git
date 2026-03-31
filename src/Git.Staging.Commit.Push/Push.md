새로운 원격 저장소 등록하기
먼저, 푸시하고자 하는 새로운 서버 주소를 별도의 단축 이름으로 등록해야 합니다. 보통 기본 저장소는 origin이라는 이름을 쓰지만, 두 번째 저장소는 backup, upstream, 또는 server2 같은 이름을 자유롭게 붙일 수 있습니다.

```Bash
git remote add <저장소이름> <저장소주소>
```
예시: git remote add backup https://github.com/username/backup-repo.git
등록이 잘 되었는지 확인하려면 git remote -v 명령어를 입력해 보세요. origin과 함께 새로 추가한 이름이 목록에 뜰 것입니다.
