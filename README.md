--------------------git--------------------------------
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

*****Installation for Git in your local laptop :
 URL- https://git-scm.com/downloads   #it support os like Windows,Linux,Mac.

yum install git -y # for linux 

After completed of installation go to cmd promt check : git --version 


git init -----to intilaise git process (Optional)

-----introduce yourself to Git-------------- 
------all commands start with git only-----------------

---------------------Git commands---------------------
----------------### Tell Git who you are----------------------------
git config --global user.name --- to check configured name 
git config --global user.email --- to check configured email

Below Example :--

git config --global user.name "veer"
git config --global user.email "cloud87777@gmail.com"



--------------------git workflow------------

git status ---- to check file will be tracked or untracked 
git add -----to add file into staging area from local working directory
git status ----to see the status of the file where it is 
git commit -m "comment"
git push 


-------------------------GITHUB------------------------------
 GitHub is one of the most popular resources for developers to share code and work on projects together. It’s free, easy to use, and has become central in the movement toward open-source software.


git clone ---- to clone entire repository in first time 

git pull ------to pull the updates and changes from repository

git push ------to push the local updates into remote repo




-----git push----- SSH ----

# push the changes by using SSH #

### To generate SSH Key

ssh-keygen (give this command into your terminal)

copy the publickey id_rsa.pub

paste into github ssh keys 

settings-->ssh and GPG keys--> Add new ssh key and give any name and paste it your publickey over there 



Note:-
If we clone a repository by using https method while push time if you want to use different method we have to remove existing https endpoint and add new  endpoint 

to check origin endpoint:      git remote -v
To remove existing endpoint:   git remote remove origin
 
To set new origin              git remote add <name> <url>


Ex: git remote add  CloudTechDevOps git@github.com:CloudTechDevOps/project0730.git 





####### Git Token method #######


# push the chnages by using GitHUb Token #

###To generate Token 

settings-->Developer settings-->personal access token -->Token classic --> generate token

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


# Example:

git push https://<token>:/user/repository.git

Examples:



git push https://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@github.com:/user/repository.git


git push https://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@github.com:/CloudTechDevOps/project0730.git


git remote add  origin https://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@github.com:/CloudTechDevOps/project0730.git






## BRANCHES:
It's an individual process of development for code.
we create individual branch in real-time to do test and developed.
each developer will work on their own branch.
At the end we will merge all branches into actual branch.
Default branch is Master or MAin.

git branch		        : to list the branches
git branch dev	                : to create a new branch
git checkout dev	        : to switch from one branch to another.
git checkout -b dev             : to create and switch from one branch to another.
git branch -m oldname newname	: to rename a branch
git branch -D dev	        : to delete a branch

benefits:


1. We can identify the issues before push into main branch

2. We can overcome git conflicts 

3. Rollback process is easy

4. code verified & approved so reduced deployment activities

