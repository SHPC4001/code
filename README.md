#How to use this repository

This repository can be used to keep track of the example programs, and easily sync them to your home folder on Magnus.

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
    
## Pushing your changes to github

To set the remote repo (not necessary if cloned):

    git remote add origin https://github.com/yourusername/repository_name.git

To push to the remote repository on github:

    git push origin master

To see the remote repos available:

    git remote -v

## Modifying files

After modifying files, check your git status:

    git status

You can then `git add` files that you want to stage manually, or do

    git commit -a

to add *and commit* all modified files.
