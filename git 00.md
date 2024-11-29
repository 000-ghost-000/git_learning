27-11-2024 , 20:29:21

# this is the notes that will contain information about the topic `git`

so let's start ...
BTW i am using Linux Debian so see the codes and commands according to the operating system

[git documentation](https://git-scm.com/doc)
[git documentation](https://docs.github.com/en/get-started/getting-started-with-git/set-up-git)
[YouTube lecture](https://www.youtube.com/watch?v=zTjRZNkhiEU&list=WL&index=2)

1. first of all we have `git status` 
	1. this command checks if the repository is already initialised or not and if it has been initialised then on which branch we are currently on 
	2. it is a best practice to use this command every-time to check where we currently are and if the repo has been already init or not to git
2. `git init`
	1. we use this command to initialise the repository to the got so that we can use the features of the git software  
	2. [[git 00.canvas|git 00]]
3. `git add`
	1. the git add command is the command that we use to tell the software that we want these files to be tracked by the git 
	2. we use the command by syntax `git add <file names>` or `git add .` this command add all the files in the directory / repository to be tracked by the git software
	3. [[git 00.canvas|git 00]]
4. `git commit`
	1. after we have successfully added all the necessary files to the git we an now save the changes by using the `git commit -m "intial commit"`
	2. the `-m` denotes that we are going to write a commit message and then we write the commit message in double quotes immediately after the `-m` 
	3. git follows the rule of atomic commits means that one commit does one job 
	4. `git commit -am "message"` this command is used to add and commit at the same time
	5. [[git 00.canvas|git 00]]
5. `git push`
	1. this command help us to push the committed code to a remote repository or a server / service like [github](https://github.com/) 
	2. [[git 00.canvas|git 00]]
---------------------------------------------------------
---------------------------------------------------------
#### everything explained above in action and with some commentary
``` markdown
To upload a repository on GitHub from the terminal, follow these steps:
Step 1: Initialize Git in your project directory (if not already done)

cd /path/to/your/project
git init

Step 2: Add your files to the staging area

`git add .`

Step 3: Commit your changes

git commit -m "Initial commit"

Step 4: Create a repository on GitHub

    Go to your GitHub account.
    Create a new repository with a name of your choice.
	Do not initialize the repository with a README file, as you'll be          pushing your existing project.

Step 5: Link your local repository to GitHub

In your terminal, run the following commands (replace <username> and <repository> with your GitHub username and repository name):

git remote add origin https://github.com/<username>/<repository>.git

Step 6: Push the code to GitHub

Run the following command to upload your local files to the remote GitHub repository:

git push -u origin master

Step 7: Verify on GitHub

Go back to the repository page on GitHub to verify that the files have been uploaded successfully.

Let me know if you need help with any of these steps!
```
---
---
6. `git log`
	1. this command is used to check all the commits done for a repo and the info about the commits like commit id , author , date & time , commit message
	2. `git log --oneline` this command will give you the important information about the commits in just one line like the commit id and the commit message
7. `git config`
	1. `git config --global` this command is use to set the config file globally so that we don't need to do this every-time we create a new repo
	2. `git config --global user.name "<name>"` this command is used to set the name for the user who is using the machine 
	3. `git config --global user.email "<email_name@domain.com>"` this command set the email for the user using the git software 
	4. `git config --global core.editor "code --wait"` this command is used to set the default code editor for the git so that if you forgot to to write the commit message by change git will open your favourite code editor "in my case i am using vs-code" and the `--wait` is used to tell the code editor to wait after opening so that we can write things in the editor and save them
8. `.gitignore`
	1. this is a file we create to mention all the files and folders we don't want our git to track
	2. like the `.env` file like these contain sensitive information and we don't want to push or to commit these files so we just add the name of the file and folder to the `.gitignore` file 
	3. for files we write `<file_name>`
	4. for folder we write `<folder_name/>` this `/` shows or tells the got software that this folder and the folders and files inside this folder are to be completely ignored and not to be tracked
9. `.git`
	1. this is the folder which is created when we initialised the repo using `git init` command 
	2. this folder contains all the necessary files and folders the software needs to keep track of the directory it is currently in
[[git 01]]