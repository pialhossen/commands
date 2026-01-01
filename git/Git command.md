Generating ssh key

     ssh-keygen -t rsa -b 4096 -C "piyal13133@gmail.com"

Activeing agent

    eval "$(ssh-agent -s)"

Creating agent file

    touch ~/.ssh/config

Creating agent file (for windows)

    ssh-add C:\Users\[Your-Username]\.ssh\id_rsa

Opening agent file

    nano ~/.ssh/config

Adding key to agent

    ssh-add ~/.ssh/id_rsa

See private key

    cat ~/.ssh/id_rsa

See public key

    cat ~/.ssh/id_rsa.pub

Connect key to github

    ssh -T git@github.com

Check git remote path

    git remote -v

Remove remote path

    git remote remove origin

File Hard reset

    git reset --hard

Go back to a commit and delete every commit after that

    git reset --hard <commit-id>

Undo a commit by creating a new commit -- keep the history of that old commit

    git revert <commit-id>

File recover

    git checkout filename

Update local
    
    git pull origin master

Update remote 

    git push origin master

Force push to remote -- may rewrite history

    git push -f

Force push only if noone has pushed since i last pushed

    git push --force-with-lease

Commit

    git commit -m "commit message"

git show different between working tree vs staging area

    git diff

git show different between previous commit vs staging area

    git diff --staged

Direct Commit

    git commit -a -m "Direct commit message"

Git delete

    git rm file.name

Git rename

    git mv currentFile.name renamedFile.name

Git Untrack

    git rm --cached <file_name>

Git repository delete

    rm -rf .git

Git alias

    git config --global alias.st "status"

Git new Branch
 
    git checkout -b branchName

Git switching Branch

    git checkout branchName 

Git show all Branch

    git branch

Git merge

    git merge branchName

Git pull and rebase (keep straight timeline) 

    git pull --rebase

Git show branch with small detail

    git branch -v

Git show merged branch

    git branch --merged

Git show unmerged branch

    git branch --no-merged

Git safe branch delete

    git branch -d branchName

Git unsafe branch delete

    git branch -D branchName

Git delete remote branch

    git push -d origin branchName

Git create a remote branch

    git push origin <branch-name>

Git create a branch from a commit

    git checkout -b <new-branch-name> <commit-id>

Git Change remote url

    git remote set-url origin [url]

Git Get remote url

    git remote get-url origin


### Replaceing master branch with another branch

```
git checkout master
git pull
git checkout ""another branch name""
git merge --allow-unrelated-histories -s ours master
git checkout master
git merge ""another branch name""
```
