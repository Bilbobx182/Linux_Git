# Gitconfig

- Used to contain my git aliases.

## Location : 
- ~/.gitconfig

## Contents

```
[user]
	name = Ciaran O Nuallain
	email = my.email@gmail.ocm
[pull]
	rebase = true
[alias]
	st = status
	ci = commit
	co = checkout
	b = branch
	rb = rebase
    rh = reset --hard HEAD^
	z = !git co @{-1}
	aa = !git ci -a --amend --no-edit
	sq = !git reset --soft master && git ci
	u = !git co master && git pull origin master && git z
	um = !git u && git merge master
	ur = !git u && git rebase master
	po = push origin HEAD
	pof = !git po -f

	# Log
	l = log --graph --abbrev-commit --date=relative
   	 lp = !git l --first-parent
    	la = !git lp --all
    	ls = !git --no-pager lp --pretty=oneline master..HEAD
```