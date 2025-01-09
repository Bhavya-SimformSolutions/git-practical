# Advanced Git Practice

## Assignment Overview :
The objective of this assignment was to get familiar with Git Flow for structured branching and to practice advanced Git operations such as **Squash**, **Reset**, **Rebase**, and **Cherry-Pick**.
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
**Squash Commit:**</br>
Combine multiple commits into one for a cleaner history.
```bash
git rebase -i HEAD~<number_of_commits>
```
**Reset:**</br>
Undo changes either by keeping them staged (--soft) or discarding completely (--hard).
```bash
git reset --soft HEAD~1
git reset --hard HEAD~1
```
**Rebase:**</br>
Update your branch with the latest changes from develop.
```bash
git checkout TP2-T1299_Project_Setup_SubBranch
git rebase develop
```
**Cherry-Pick a Commit:**</br>
Apply a specific commit from another branch.
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
