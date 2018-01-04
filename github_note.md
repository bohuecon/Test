# set up a repository on github

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

# work flow: staging, commit, pushing
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

# tagging

# branching
```bash
git branch  # list branches
git branch b1 # adding new branch
git checkout b1  # switch to new branch, and you can modify codes, and it will not change anything on other branches

```