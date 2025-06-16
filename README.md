# basic-commands-in-terminal
This is a repo for me to have the basic or fundamental command i will use like in git, conda etc

**Create a env using conda and then activate that env**:<br>
```
conda create -n gpu-ai python=3.10 #gpu-ai is the name i give
conda activate gpu-ai
```

**Push your work in GitHub to a branch**<br>
```
1. 'cd' to that folder
2. 'git init' # initialize git
3. 'git checkout -b your-branch-name' # Create a new branch
4. # Create a file named .gitignore and list the exact filenames you want to ignore, one per line
5. 'git add .' # Stage everything
6. 'git commit -m "the-commit-message"' # and commit
7. 'git remote add origin <URL>' # Link to your GitHub repo (replace <URL> with your repo’s clone URL)
8. 'git push -u origin TP2_FedProx' # and push to the local branch name
```
**Instead want to push to the main branch**<br>
```
git checkout main
git add .
git commit -m "Your commit message"
git push origin main

```
**push new changes to the same branch after making modifications**<br>
- Just add → commit → push (no need to re-run git remote add or git init again)
```
1. Make your changes (edit/add/delete files)
2. git add .  #Stages all modified/new files
3. git commit -m "Your new commit message"
4. git push origin <Push-to-the-same-branch> # -u only for the first time push
(or) git push #git will remember the last branch as the default push target
```
**Extra Tips**
```
git status #Shows branch + file changes (imp)
git branch #list of branches
```

**Clone or Download a GitHub repository**<br>
```
1. 'cd folder-path' #Navigate to the folder where you want to clone the repo
2. Clone the repository by Copy the HTTPS or SSH URL eg. git clone https://github.com/username/repo.git
```

**Already push wrong folder or files**<br>
```
# The folder was already tracked by Git before you added it to .gitignore
# Git only ignores new untracked files - once a file/folder is committed, .gitignore won't affect it
1. git check-ignore -v folder-name/ #Verify it's actually being tracked (If no output, it's being tracked)
2. git rm -r --cached folder-name/ #Remove it from Git tracking (but keep locally)
3. Update that in your .gitignore
4. Commit and push
$ git add .gitignore
$ git commit -m "your-msg"
$ git push
```

**Show hidden files in MacOS**<br>
```
https://news.trendmicro.com/2018/03/12/how-to-show-hidden-files-and-folders-on-your-mac/ #website
```
