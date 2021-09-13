*TODO*

---
- [x] Cloning existing
- [x] Pushing local repo
- [x] branching
- [ ] Merging / Rebasing
- [ ] Pull requests
- [ ] Forks	
---
##  Clone Existing
 Run the following in the required folder
 
`git clone [URL-TO-REPO]`

## Pushing Local repo to remote

Run in the project folder

`git init`

Push to remote url

`git remote add origin [URL-TO-REPO]`

## Branching

Create new branch on local

`git branch [BRANCH-NAME]`

Switching to branch <sub><sup>(branch is local only)</sup></sub>

`git checkout [BRANCH-NAME]`

Switching to branch <sub><sup>(branch is remote)</sup></sub>

```
git pull
git checkout [BRANCH-NAME]
```

Push local branch to repo

```
git checkout [BRANCH-NAME]
git push origin [BRANCH-NAME]
```

## Merging
