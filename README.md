# Basics of Git

For learning purposes, I initially created two files, namely `index.html` and `app.js`.

## Overview

### Step 1: Git Initialization
**Commands Used:**
```bash
git init
```

### Step 2: Git Configuration
**Commands Used:**
```bash
git config --global user.name "name"
git config --global user.email "abc.email@example.com"
```

### Step 3: Staging and Committing
After learning more about the working directory and staging area, I made changes in `index.js` and applied the following git commands:

**Commands Used:**
```bash
git status  # to check the status of my repository, showing changes to be committed and also untracked files
git rm --cached index.html  # which will restore index.js to its original form and discard the changes
```

After this, I learned various ways to add files into the staging area:

**Commands Used:**
```bash
git add index.html  # which will add only index.html into the staging area
git add *.html  # which will add all the files with .html extension into the staging area
git add .  # which will add all the files in the project folder into the staging area
```

After playing with the above commands, I learned how git moves files from the staging area into the local repository with the help of various commands.

**Commands Used:**
```bash
git commit -m "Commit Message"  # which will move the files present in the staging area into the local repository
```

### Step 4: Branching and Merging
Moving to some advanced git concepts, I learned how branching works and how it is an important aspect of git. I created a new branch and tried various git commands.

**Commands Used:**
```bash
git branch Second-branch  # which will only just create a new branch
git checkout Second-branch  # which will change the branch from master to Second-branch
```

After changing the branch, I created a new file `login.html` and committed the changes made in it into the `Second-branch`. The important concept I saw was when I switched to the master branch again, the `login.html` file was not visible as it is committed in `Second-branch`. So this clears the picture in my mind that how branching can be used to work on various features on the same project at the same time.

At last, I learned how to merge two branches after completing and verifying changes.

**Commands Used:**
```bash
git merge Second-branch  # which will merge Second-branch into master
```

### Step 5: Pushing and Pulling
After working with the local repository, branching, and various git commands, I learned how to move the changes from the local repository into the remote repository on GitHub. So I created this repository on GitHub and also learned the following git commands.

**Commands Used:**
```bash
git remote  # which will show the list of remote repositories added if any
git remote add origin https://github.com/username/repo-name.git  # which will connect the repository created through a remote named origin
git push -u origin master  # which will push all the files from local to remote GitHub repository
```

## Conclusion
Through this exercise, I gained a solid understanding of the basics of Git, including initialization, configuration, staging, committing, branching, merging, and pushing/pulling to a remote repository. These skills are fundamental for version control and collaborative development in any project.
