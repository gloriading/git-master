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
