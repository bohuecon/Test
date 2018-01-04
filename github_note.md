# 1. Set up a repository on github

## method 1
1. set up a repository on Github
2. clone it to your local directory with git clone
```bash
git clone git@github.com:bohuecon/Test.git
```


## method 2
1. set up a repository on Github
2. in the local directory, set up git
```bash
git init
git add -A
git commit -m "Initial Project Version"
git remote add origin https://
git push origin master
git remote -v
```

# 2. Work flow: staging, commit, pushing
1. Stage
```bash
git add -A
git add filename.
```
2. Commit
```bash
git commit -m "message"
```
3. Push
```
git push
```

# 3. Tagging

```
git tag v1.0  # create a tag
git tag -a v1.1 -m "tag for release version 1"  # create annodated tag
git tag  # list tags
git push origin v1.0 # push tags to remote repository
git push --tags # push all tags
git tag -d v1.0
```


# 4. Branching

Notice all these set ups about branches are local, and it is not related to the remote repository. 

```bash
git branch  # list branches
git branch b1 # adding new branch
git checkout b1  # switch to new branch, and you can modify codes, and it will not change anything on other branches

# some work in branch b1
# now you have two branches, and they are of different files, if you checkout back to master, you will find the file you are editing are different. 

git checkout master
git merge b1  # return to master branch and bring up the changes in b1

git checkout b1
# git add . git commit git push you need to set up the branch online (upsstream)
git push --set-upstream origin b1
# then you can also merge online
```
