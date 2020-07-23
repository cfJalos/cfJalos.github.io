[Home page](https://cfjalos.github.io/cfJalos.github.io-reading-notes-/)

## Intro to Git##

### WHAT IS GITHUB? ###

**HISTORY**

* Originally launched as Logical Awesome in 2008; launch GitHub product later that year.
* Previously: no place on the web to publish and pull code from for open source projects.
* Had version control, but only locally.
* Rapid adoption by enterprise companies between 2009-2013. 
* June 2018: Microsoft announces acquisition of GitHub for $7.5 billion dollars. 


### WHY GITHUB ###

Centralized Version Control - before GitHub, only git available locally on computers. Cost of centralizing git very high to companies/teams. 
Open Source - no very easy/collective place on contribute to projects/programs. No public place to display code.
Networking/Employment - no place for programmers to demonstrate code/contributions, or have code reviewed.
Code review for teams - no place to review code that was decentralized. 


### WHAT IS GIT ###

Version control software - local and on the command line
Easy to install and maintain; very simple program to run.

### Default Text Editor ###
Without configuration of a default text editor, Git will use the system’s default editor–most likely Vim. To configure a different text editor, such as Emacs, type the following into your Terminal or Command Line:
* $ git config --global core.editor emacs


### Check Settings ###
To check settings, use the git config --list command.

### Getting Help ###
There are three ways to get more information on a particular command, by accessing the manual:
* git help command

* git command --help

* man git-command

### Setting up a Git Repository ###

### Importing ###
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directoryExample:
* I $ cd test (cd = change directory)
Use the git init command$ git init Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced. 
To start tracking these repository files, perform an initial commit by typing the following
* I $ git add *.c
* $ git add LICENSE
* I $ git commit -m “any message here”
Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:
$ git clone https://github.com/test

### Workflow ###

Local Repository Structure
The local Git repository has three components
* Working Directory: The actual files reside here.
* Index: The area used for staging
* Head: Points to the most recent commit
* 
### Saving Changes ###
All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.
Tracked
Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
Untracked
Untracked files were not in the last snapshot and do not currently reside in the staging area.

### The Life Cycle of File Status ###
* After you edit a file, Git flags it as modified because of changes made after the previous commit.
* You stage the modified file.
* Then, you commit staged changes.

### Check File Status ###

To determine the state of files, utilize the git status command:
* $ git status.

### Staging files ###
From the project folder, we can use the git add command to add our files to the staging area, which allows them to be tracked.
We can add a specific file to the staging area with the following command:
* git add file.js
To add multiple files, we can do this:
* git add file.js file2.js file3.js
Instead of having to add the files individually, we can also add all the files inside the project folder to the staging area:
* git add .
By default, this adds all the files and folders inside the project folder to the staging area, from where they are ready to be committed and tracked.

### Committing a File ###
After staging one or multiple files, you should commit the changes and record what you did within the commit message:
* $ git commit -m “made change x,y,z”

### Committing All Changes ###
* $ git commit -a
This command commits a snapshot of all modifications to tracked files in the working directory.

### Pushing Changes ###
Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.
Example:
* $ git push origin master
This command pushes changes from the local “master” branch to the remote repository named “origin”.

### Stashing Changes ###
When you are not ready to commit changes but do not want to lose them either, *git stash* is a great option. This command temporarily removes changes and hides them, giving you a clean working directory. When you are ready to continue working on the changes, simply use the *of git stash apply* command to retrieve the hidden changes.

### Remote Repositories ###
In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.

### Cloned Repositories ###
As mentioned earlier, for cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

### Seeing Your Remotes ###
By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.
By using git remote -v, you can view all the remote URLs next to their corresponding short names.
$ cd example

* $ git remote -v

