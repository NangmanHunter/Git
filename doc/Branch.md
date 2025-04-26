# Branch


## BranchType
Branch
- LocalBranch
- RemoteBranch

Alias
```
LocalBranch 👉Branch
RemoteBranch👉RemoteBranch
```
## BranchList
- ```
  git branch
  ```
## BranchStauts
- ```
  git status
  ```


## BranchCreate
- git branch 🪜...
## BranchRemove
- git branch -d 🪜...
- git branch -delete 🪜...


```shell
git branch -delete 🪜...
```
## BranchMove
- git checkout 🪜...
- git switch 🪜...
## BranchMoveCreate
- git checkout -b 🪜...
- git switch -c 🪜...


## BranchPush
- git push origin 🪜...


## CommitCreatePush
```
CommitCreatePush
Commit▶️Create▶️Push
Commit▶️BranchCreate▶️BranchPush
```


Commit
- git add .
- git commit -m "bac"

BranchCreate
- git branch 🪜...

BranchPush
- git push origin 🪜...
## CommitCreatemovePush
```
CommitCreatemovePush
Commit▶️Createmove▶️Push
Commit▶️CreateMove▶️Push
Commit▶️BranchCreatemove▶️BranchPush
Commit▶️BranchCreateMove▶️BranchPush
```


Commit
- ```
  git add .
  git commit -m "bac"
  ```

CreateMove
- git branch -b 🪜...

Push
- ```
  git push origin 🪜...
  ```

## RemotebranchRemove
```
RemotebranchRemove
RemoteBranchRemove
Remotebranch Remove
RemoteBranch Remove
```

RemoteBranchRemove
- ```
  git push origin --d 🪜...
  ```
- ```
  git push origin --delete 🪜...
  ```

