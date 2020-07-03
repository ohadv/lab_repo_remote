This is an example of README.md

#Git init:
$ git config --global user.name "full name"
$ git config --global user.email x@x.x 
$ mkdir lab_repo  (to remove the directory: rm -r ...)
$ cd lab_repo  (backward: cd -, root: cd )
$ git init
$ git status

	# Some editing:
	touch .gitignore => vim .gitignore => Insert=> (somefile\n/somedir\n)  => Esc+ :wq
	$ vim zen_of_python  
	$ ls |  $ ls -a  (directory content)

# add / commit 
git add . (. = all, expect files / directories listed in .gitignore), can specify file name instead of .
git commit -m "some msg"

	# restore 
	$ git restore "file_to_restore"  # restore commited file

# branch 
$ git branch login # create new branch
$ git checkout login  # Switched to branch 'login'
$ git checkout master  # Switched to branch 'master'
$ git merge login    #  Merge login  (called from master), Files created by login, available to master


# remote
$ git remote add origin https://github.com/ohadv/lab_repo_remote.git
$ git remote  # returns "origin"
$ git push -u origin master   # upload repository (master will be accessable in github, Branch 'master' set up to track remote branch 'master' from 'origin'. use -f to force the push.

	# README file
	$ touch README.md  # create readme file
	$ vim README   # edit ...
	$ git add .
	$ git commit -m "commit README"

# utils
$ clear   # bash will be cleared
$ git rebase -i HEAD~6  # handle prev. commit.






