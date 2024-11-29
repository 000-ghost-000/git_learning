28-11-2024 , 22:47:14

10. `git branch`
	1. this command will tell us on which branch we are currently on using the concept of pointer
	2. it shows all the branches that are available
11. `git branch <name of branch>`
	1. this command is used to create new branch so that we can perform multiple actions on the code without affecting other branches or the  main code base
	2. `git branch -M <branch name>` this command is used to rename a branch
12. `git checkout <name of branch>`
	1. this command is used to change the main branch , the pointer which is pointing to some branch
	2. `git checkout -b <name of branch>` this command creates the branch and move the head / pointer to that branch
	3. `git checkout HEAD~2` this command tells us we want to go two commits back from where our head is currently
	4. `git checkout <hash>` this command is used to go to particular commit or branch by providing the hash
	5. `git checkout master` after we have moved back in commits when we have to come back to the place we were we use this command 
13. `git switch <name of branch>`
	1. same as the `git checkout <name of branch>`
	2. `git switch -c <name of branch>` this command creates the branch and move the head / pointer to that branch
	3. always commit before switching to a new branch
14. `git merge <name of branch>`
	1. to merge some branch i have to be on the branch i want the other branch to merge into
	2. like for example i want to merge a branch named `nav-bar` to my `master` branch , so i should have my pointer pointing to master and then use the `git merge nav-bar` command to merge two branches
15. `git branch -d <name of branch>`
	1. this command deletes the branch 
16. conflict while merging
	1. when two or more branches change the same file and after merging the file we have to remove the conflicts manually 
	2. when writing the `git merge <branch>` command of there is a conflict the terminal will tell us that there is a conflict occurring and we then have to remove that conflict manually in the IDE 
	3. after resolving the conflict and adding and deleting the codes we need and don't need we then do a `git commit -m "message for commit"` to commit this changes we made and merge the branch successfully 
	4. we remove the `<<<<head ` and then ===== and then `>>>>branch` we add and delete the code we wanted to keep and delete 
17. `git diff`
	1. this command help to compare the same file in different commit times
	2.  `git diff --staged` this command is used to compare the file at different times of adding
	3. `git diff <commit 1> <commit 2>` this command is used to compare files in two different commits in `commit 1` and `commit 2 ` we provide the commit id also known as the SHA id , another way of using the same command is `git diff <commit 1>..<commit 2>`
	4. `git diff <branch 1>..<branch 2>` this command is used to compare two different branches
	5. we can interchange the commit 1 and commit 2 places 
18. `git stash`
	1. without committing or stashing the files git don't allow us to change branches cause our files may be overridden in other branch 
	2. `git stash` this command help us to stash our code and files so that we can change branches without committing our code
	3. `git stash pop`  this command is used when we are back to our branch and we want our files in the same way as we stashed them we use this command 
	4. stash is not just limited to one branch we can stash a file in one branch and can pop that same file in other branches too
	5. `git stash list` this command gives me all the information about all the files which are being stashed 
	6. `git stash apply <stash name>` this command is used to apply specific stash specific stashed files into the branch
19. `git resore <file name>`
	1. this command is used to restore the file as it was in the last commit

[[git 02]]