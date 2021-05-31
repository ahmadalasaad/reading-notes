# Git

## What is git?

* Git is a distrebuted version control system that stores data in a file system made up of snapshots.
* Mostly relies on local operations because most necessary information can be found in local resources.
* Every single change applied to any file or directory is tracked by Git.
* Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. 
* Files in Git can reside in three main states: committed, modified and staged.

## Getting started

* [click here](http://git-scm.com/download/) to go to download pages

Git includes inherent Graphical User Interface (GUI) tools

* You can access a variety of GUI clients [here](https://git-scm.com/downloads/guis)

* After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.

Type the following into Terminal or Command Line:

git config --global user.name "Ahmad Alasa'd"

git config --global user.email "example@email.com"

To confirm that you have the correct settings, enter the following command:

git config --global user.name (should return Ahmad Alasa'd)

git config --global user.email (should return example@email.com)
