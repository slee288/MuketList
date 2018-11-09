##Git and Github are VERY different
* Git is technology
* Github is an application that WORKS with Git
* 

##Git
* At the end of project, I will end up with lots of committs
* 

## Git init:
* To get git going, use "git init" command
*   - if you see (master), it is a sign that git is initialized
*   

## 3 States of Git
*   
*   - Working Directory (everything that we are working on)
*       Area where all of our files and directories and changes are 
*       living all the time
* (Git is constantly listening for changes)
*   
*   - Staging Area
*       - Files and directories that we explicitly add to the stating area
* (If we want to explicitely track something (staging area) we add
* those files into staging area)
*   
*   - Git Repository
*       -Where all our snapshots are stored
* (Once we add those files to the staging area, we commit those files to
* another area, called repository)
*   

##Git add
* The file has been changed, but git repo does not know anything about it
* This is where we put files into the staging area
* Added files show up in green letters
*   - Use git add *.filetype in order to add all the files with same extension
*   - Use git add -A adds ALL files and folders from the directory that I am in
* 


##Git status
* Tracks which files has been changed, or added in the current directory
* Recommended to be used between any time to keep track of the files
* 

##Git commit
* Commits those files that are in staging area into actual repository
* -m is a flag which means a message in here
* Once committed, no files show up in the staging area
* 

##Git log
* Checks the history of what snapshots we have created so far
* This history will also display the message that I have written
* 

##Git reset
* If we don't want certain files to be in the commit, we use this command
* "git reset HEAD <file>"   
*   => this specific file will be removed from the staging area
*   

##Git ignore
* First, we create .gitignore file in the current directory
* Then, we add name of the file to ignore
* If we do all this, git will NOT track the file that is written inside
* .gitignore file, and it will not even show up in "git status" command
* Yet, it will be possible to add the .gitignore file when we explicitly add it
* 

##Git Branches
* Master branch is the main branch by default
* "git branch" shows all the branches that I have
*   - "Master" is the branch that comes by default
*   

##Git checkout
* "git checkout -b <name>" will create the new branch by the name declared,
* and we move into that branch
* 
* "git checkout <name>" will switch to the branch with that name
*   - If we are already inside that branch, git will say "Already on <name>"
*   

##Branch Merging
* Let two branches be separate (one master, one feature)
* If we commit files inside feature branch, it will not show up in 
* master branch log
* Same applies when we commit files in master; such commits will not
* show up in feature branch log
* 
* This is where "git merge <name>" comes in
* This can be done on a main branch, and merging the new branch onto it
* Once we have done this, master branch will recognize changes 
* made in feature branch
* If we make new changes in feature, we can merge the branch again to the 
* master
* 

##Remove Branch
* "git branch -d <name of branch to delete>"
* If I check branches after, removed branch will no longer exist
* Yet, we still have changes brought by the deleted branch
* 


##Uploading to GitHub
* "git remote add origin https://github.com/slee288/yelpcamp.git"
* "git remote -v"   -> checks if uploaded to correct url
* git push -u origin master -> pushes the current repo to github repo






