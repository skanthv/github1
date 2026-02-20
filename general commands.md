# create a copy of github repo in your local pc and link to the github repo (i.e. clone)
git clone github-repolink.git

open the repo folder in vscode

# know current branch
in left bottom, see the current branch name, click it to change to different branch
or in terminal type `git status` to know the current branch

# to create new branch and switch to it
`git branch -b new-branch-name`
`git branch -b feature/newfeature`

# making code changes and adding those changes to github
check the branch you are now currently in..if that is where you want to change code, do it..save
## stage the changes
`git add .` to stage all changes done
## commit the changes to local git repo
`git commit -m "msg"` 
## push changes to the github repo , but to the new branch that you created locally
Because you initially cloned the repo, so the link to it is still there so 
`git push` . auto creates  a branch as in your local, pushes code to the remote repo 

### if you did not clone the repo from github, and you only created a github repo later after creating the code locally..
you need to first link the github repo to the local git repo
`git remote add origin github-repo-link.git`
then `git push origin local-branch-name` this adds contents in current git branch in local code to github repo's branch same as local branch .


# adding the changes to the main branch in github
go to azure devops, go to pull requests option on the left side on the repo, fill the form
indicate the branch you created, which branch you want to merge into, give details and submit
