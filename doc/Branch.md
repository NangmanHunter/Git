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
- ```bash
  git branch
  ```
## BranchStauts
- ```
  git status
  ```


## BranchCreate
- ```bash
  git branch 🪜...
  ```
## BranchRemove
- ```bash
  git branch -d 🪜...
  ```
- ```bash
  git branch -delete 🪜...
  ```


```bash
git branch -delete 🪜...
```
## BranchMove
- ```bash
  git checkout 🪜...
  ```
- ```bash
  git switch 🪜...
  ```
## BranchMoveCreate
- ```bash
  git checkout -b 🪜...
  ```
- ```bash
  git switch -c 🪜...
  ```


## BranchPush
- ```bash
  git push origin 🪜...
  ```


## CommitCreatePush
```
CommitCreatePush
Commit▶️Create▶️Push
Commit▶️BranchCreate▶️BranchPush
```


Commit
- ```bash
  git add .
  ```
- ```bash
  git commit -m "bac"
  ```

BranchCreate
- ```bash
  git branch 🪜...
  ```

BranchPush
- ```bash
  git push origin 🪜...
  ```
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
- ```bash
  git branch -b 🪜...
  ```

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

