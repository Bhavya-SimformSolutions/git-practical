# Advanced Git Practice

## Commands Used

### Initialize Repository and Git Flow
```bash
git clone <repository-url>
cd <repository-name>
git init
git flow init
```
### Create Feature Branch
```bash
git flow feature start TP2-T1299_Project_Setup
```

### Create Sub-Branch
```bash
git checkout -b TP2-T1299_Project_Setup_SubBranch
```

### Perform Git Operations
**Squash Commit:**
```bash
git rebase -i HEAD~<number_of_commits>
```
**Reset:**
```bash
git reset --soft HEAD~1
git reset --hard HEAD~1
```
**Rebase:**
```bash
git checkout TP2-T1299_Project_Setup_SubBranch
git rebase develop
```
**Cherry-Pick a Commit:**
```bash
git cherry-pick <commit-hash>
```

### Push Branches to GitHub
```bash
git checkout develop
git push -u origin develop

git checkout TP2-T1299_Project_Setup
git push -u origin TP2-T1299_Project_Setup

git checkout TP2-T1299_Project_Setup_SubBranch
git push -u origin TP2-T1299_Project_Setup_SubBranch
```

### Pull Request and Merge
**1** : Create a PR from TP2-T1299_Project_Setup_SubBranch to TP2-T1299_Project_Setup. </br>
**2** : Merge the PR after review.</br>
**3** : Create a PR from TP2-T1299_Project_Setup to develop. </br>
**4** : Merge the PR after review.
