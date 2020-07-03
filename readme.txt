1.Keep .gitignore in project directory, and modify it regulary
2. Create branch by $ git branch. For example: git branch login

3. This line was edited after switching from branch login.
The file login.txt that was created from login branch, no
longer shown in lab_repo directoty after checkout ($ git checkout master)

4. To merge login so that the login.txt can be edited from master branch
use $ git merge login (login is the name  of  the branch to be merged)

5. Now  after merging go to github.com for remote repository. Sign in to github

6. Create the repositort : lab_repo_remote => $ git remote is still none.
=> Use:$ git remote add origin https://github.com/ohadv/lab_repo_remote.git
=> Now git remote will return origin.
Afterward, use git push -u origin master, to setup branch master to track remote branch master
from origin
