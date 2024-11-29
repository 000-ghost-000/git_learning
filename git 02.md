29-11-2024 , 13:55:47

20. `git rebase <branch>`
	1. this command can be used as a alternative way of merging
	2. this command can be used as a cleanup tool
	3. this command is not meant to be run on the main or the master branch 
	4. if there is a conflict while using the command we have to manually remove the conflicts 
### GitHub
* go to GitHub and create a new repo
*  GitHub is a service that help us to maintain our code in an online cloud location
1. `git clone <URI>`
	1. this command is used to clone a repo locally from GitHub 
2. `git remote`
	1. `git remote -v` this command help us to check if there is any repo being set up remotely 
	2. `git remote add <name> <URI>` we can add out repo that we have created on GitHub by writing its URI in the placeholder and we can prove a name too like GitHub uses `origin` as it's default name
	3. `git remote rename <old> <new>` this command is used to rename the `origin`
	4. `git remote remove <name>` this command is used to remove the `origin` 
3. `git push`
	1. `git push -u origin <name>` this command is used to push the code and files to GitHub , `git push <remote name> <branch name>`
	2. the `-u` in the `git push -u ` is uses to set the branch as the upstream branch means we don't have to write branch name every-time we push , we just have to do a `git push` and that's it 
4. `git fetch`
	1. this command is used to bring the latest modified code from GitHub to local repo but not to your working area
5. `git pull`
	1. this command brings the latest code to your working area
	2. `git pull` = `git fetch` + `git merge`

### readme.md

this is the file we create as the documentation of the code we have written and the work we did

### open source

