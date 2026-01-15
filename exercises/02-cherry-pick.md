# Exercise 02: Cherry-pick

## Goal
Bring a single bugfix commit from one branch onto another branch without merging everything.

This simulates applying a hotfix from another branch.

---

## Start here
```bash
git switch exercise/cherry-target-start
git switch -c student/<yourname>-cherry
```
## Task
1. Inspect the source branch commit history:

```
git log exercise/cherry-source --oneline
```


2. Identify the commit with the message:

"fix: important bugfix"


3. Cherry-pick that commit onto your current branch:

```
git cherry-pick <commit-hash>
```

## Expected output
- git log --oneline -5 shows the bugfix commit on your branch

- The file src/cherry.txt includes the bugfix content
