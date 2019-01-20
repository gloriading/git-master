# GIT PLAYGROUND 🤘

## Settings

* Set git default editor to VScode:

  ```
  git config --global core.editor code
  ```

* Edit config file with text editor:

  ```
  git config --global -e
  ```
* Set global user & email:

  ```
  git config --global user.name "Jane Doe"
  git config --global user.email "jane@gmail.com"
  ```

* See what are in the config file

  ``` 
  git config --list 
  ```

* Set Alias for git commands
  ```
  git congit --global alias.cc checkout
  git config --global alias.br branch
  git config --global alias.l "log --oneline"
  git config --global alias.g "log --oneline --graph"
  git config --global alias.ls 'log --graph --pretty=format:"%h <%an> %ar %s"'
  ```

## Everyday Git

* Update current branch
  ```
  git pull
  ```
* Create a new branch
  ```
  git branch new_branch
  ```
* Creata and Go to a new branch
  ```
  git checkout -b new_branch
  ```
* Stage your all your changes
  ```
  git add .
  ```
* Stage one change only
  ```
  git add fileName
  ```
* Create a commit message in terminal
  ```
  git commit -m 'My first commit message' -m 'More description'
  ```
* Create a commit message in a text editor
  ```
  git commit 
  ```
  An editing screen will pop up.
  Put commit messages there, save, and close.
* Stage and Commit 
  ```
  git commit -am 'your commit message'
  ```
* List all local branches
  ```
  git branch
  ```
* List all branches (local and remote)
  ```
  git branch -a
  ```
* Push a local branch to remote
  ```
  git push --set-upstream origin my_branch
  ```
  or
  ```
  git push -u origin my_branch
  ```


## Redo commits

* Check the log 
  ```
    git log --oneline

    You see: 
    e12d8ef (HEAD -> master) add apple.html
    85e7e30 add description in banana.txt
    657fce7 add banana.txt
    abb4f43 update index page
    cef6e40 create index page
    cc797cd init commit
  ```

* If want to redo last commit - method 1: use `reset` (i.e. go to)

  ```
    git reset HEAD^
    or
    git reset 85e7e30 
  ```

* After going to previous commit, but regret that, how to get back to head?
* use `git reflog` to check SHA, then use `git reset SHA`  go back

## Need to switch to other branch while in the middle of something?

* commit current work 
* go to other branches to do stuff
* go back to previous working branch - `git reset HEAD^`

## TAG
* Create a tag

  ```
  git tag -a v1.4 -m "my version 1.4"
  ```
* Delete a tag
  ```
  git tag -d v1.4
  ```
* Checkout a tag
  ```
  git checkout v1.4
  ```
* Show tag definitions
  ```
  git tag -n
  ```
* List all tags
  ```
  git tag
  ```

### READ THIS:
https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
