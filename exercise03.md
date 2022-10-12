# Exercise 3 - Configuring your first repository

1. Enable color

        git config --global color.ui auto

2. Set your name

        git config --global user.name "John Doe"

3. Set your email address

        git config --global user.email "john.doe@somewebsite.com"

4. Why did we use the `--global` flag?  (What does that do?)
   So that it applies to only that one user (and not all) on the system.


5. Check your git config to show the changes you have made

        git config -l

For more information, check out [Customizing Git Configuration](https://www.git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)

On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
(base) ulisesmarian@Ulisess-MacBook-Air my_repository %  git config --global color.ui auto
(base) ulisesmarian@Ulisess-MacBook-Air my_repository %  git config --global user.name "Ulises Marian"
(base) ulisesmarian@Ulisess-MacBook-Air my_repository %  git config --global user.email "ulises.marian@hotmail.com"
(base) ulisesmarian@Ulisess-MacBook-Air my_repository %  git config -l
core.excludesfile=~/.gitignore
core.legacyheaders=false
core.quotepath=false
mergetool.keepbackup=true
push.default=simple
color.ui=auto
color.interactive=auto
repack.usedeltabaseoffset=true
alias.s=status
alias.a=!git add . && git status
alias.au=!git add -u . && git status
alias.aa=!git add . && git add -u . && git status
alias.c=commit
alias.cm=commit -m
alias.ca=commit --amend
alias.ac=!git add . && git commit
alias.acm=!git add . && git commit -m
alias.l=log --graph --all --pretty=format:'%C(yellow)%h%C(cyan)%d%Creset %s %C(white)- %an, %ar%Creset'
alias.ll=log --stat --abbrev-commit
alias.lg=log --color --graph --pretty=format:'%C(bold white)%h%Creset -%C(bold green)%d%Creset %s %C(bold green)(%cr)%Creset %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
