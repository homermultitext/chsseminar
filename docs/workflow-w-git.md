---
title: The HMT workflow with git
layout: page
---


## Summary

Your regular work cycle is:

1.  git pull
2. (do a little work)
3.  validate+verify in sbt console
4.  git add FILENAME
5.  git commit -m "MESSAGE"
6.  git push


## Notes on `git`


`git status` is a good way to see whether anything in your repository has changed


### In your regular workflow

`git pull` = "bring down changes from the shared repository"

`git add FILENAME` = "add a file to the list to save locally"

`git commit` =  "save files on the list in your local copy of the repository"


`git push`  = "send your locally saved changes back to the shared repository"
