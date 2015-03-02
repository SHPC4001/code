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

Do this either in a new directory or a current directory

To add files to the repository:

    git add files_to_add

To commit your changes:

    git commit -m "Message"

After modifying files, check your git status:

    git status

You can then `git add` files that you want to stage manually, or do

    git add --update

to add all modified files.

To set the remote repo (not necessary if cloned):

    git remote add origin https://github.com/yourusername/repository_name.git

To push to the remote repository on github:

    git push origin master

To see the remote repos:

    git remote -v