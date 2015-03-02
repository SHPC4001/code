#How to use this repository

This repository can be used to keep track of the example programs, and easily sync them to your home folder on Magnus. [Online git reference](http://gitref.org/branching/).

##Setting up Git

To set your username and github email:
    git config --global user.name "Your Name Here"
    git config --global user.email "your_email@youremail.com"

##Cloning this repository
    git clone https://github.com/SHPC4001/code.git

You can then check for updates with 
    git pull

##Making your own repo

To make a repo from scratch:
    git init

Do this either in a new directory or a current directory. Then, to add files to the repository:
    git add files_to_add

Commit your changes to add them to the 'staging area':
    git commit -m "Message"
    
### Pushing your changes to github

To set the remote repo (not necessary if cloned):
    git remote add origin https://github.com/yourusername/repository_name.git

To push to the remote repository on github:
    git push origin master

To see the remote repos available:
    git remote -v

### Modifying files

Delete files:
    git rm <filename>

Move files:
    git mv <filename>

After modifying files, check your git status:
    git status
    git status -s

You can then `git add` files that you want to stage manually followed by a `git commit`, or do
    git commit -a

to add *and commit* all modified files.

### Viewing and reverting file changes

View file differences that have not yet been staged:
    git diff <filename>

View file differences that have been staged:
    git diff --cached <filename>

View file differences that have not yet been committed:
    git diff HEAD <filename>

Keep local changes, but remove from the staging area:
    git reset HEAD <filename>

Revert a file to previous commit (i.e. undo *all* local changes):
    git checkout -- <filename>

Unstage files AND undo any changes in the working directory since last commit:
    git reset --hard HEAD

Revert *all* local changes and commits, and return to the remote copy:
    git fetch origin
    git reset --hard origin/master

### Updating your repo from your remote copy on github:

    git pull

