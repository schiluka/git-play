# Playing around git branching

## Useful commands

## Basic
git add hello.py
git commit -m "init commit"
git push
git status
git pull
git diff branch1 branch2
git diff --stat --color master..branchName
git diff master..release3

## Branches
git checkout -b release1
git branch
git add rel1.py 
git commit -m 'release1 changes'
git push --set-upstream origin release1

git checkout -b release2
git branch
git add hello.py rel2.py 
git commit -m "release2 changes"
git push --set-upstream origin release2

## Merges
git checkout master
git branch
git merge release1
git status
git push
git status
git branch -d release1

## Tags
git log
git tag 1.0 <commitId>
git push --tags origin

## Rollback
git reset --hard <commitid>
git reset --hard HEAD~1 --will get you back 1 commit
git reset --hard origin/master --ignore local changes

