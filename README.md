# VERSION CONTROL WITH GIT
I found the following commands and steps useful in version control

## Initializing git
Create a directory on your computer and navigate to it
	`mkdir new-git-repo && cd new-git-repo`
	`git init`
	`ls -la`
You should notice a .git file in the directory

## Add files and add them to stage phase
- Add the files containing code to the directory.
- check the status of commits. This will display all the changes that have occured yet not staged.
	`git status`
- Stage files to be committed:
	`git add <file-name>`
- Alternatively, to add all the files:
	`git add .`
  
## Making commits
- Make an initial commit with a flag for the message:
	`git commit -m 'initial commit'`
-Alternatively run commit without a flag.The code editor pops up and you 
can add a commit message:
	`git commit`

## Create a branch
- To create a branch:
	`git branch backup`
- To move to the branch:
	`git checkout backup`
- To merge changes between braches:
	`git checkout <branch-to-be-merged-in>`	
	`git merge <branch-to-be-merged>`

## Reverting a commit
- To revert a commit, first identify the SHA of the commit for reference:
	`git log --oneline`
- Copy the 7 digits showing up in front of the message and reference the in the revertion:
	`git revert *******`

## Push changes to a remote repository
- Create a repository on github and identify the HTTPS link address
- Push the source code:
	`git branch -M main`
	`git remote add origin https://github.com/username/repositryname.git`
	`git push -u origin main`

