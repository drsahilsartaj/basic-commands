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
