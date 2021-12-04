# Introduction to Git
An introduction to Git, Version Control and GitHub


## Contents
1. What you'll need before you start
2. Version Control
    1. What is the purpose of version control?
    2. What are the core components of version control?
    3. What is Subversion and Git
3. How Git works
    1. Phrases
    2. Exploring things in GitHub
    3. Clone, Change, Commit, Push
    4. Seeing the difference
    5. Make a mistake - undo the change
    6. Merging Changes
4. Github Features
    1. Using branches
    2. Using pull requests
5. Terminology Wrapup


## What you'll need before you start
  1. Install Git ([windows](https://git-scm.com/download/win) | [mac](https://git-scm.com/download/mac))
  2. Install [Visual Studio Code](https://code.visualstudio.com/) or use a text editor of your choice
  3. A Github Account ([sign up](https://github.com/signup) | [sign in](https://github.com/login))


## Version Control
This section takes you through what version control is used for and some of the core components and technologies used for it.


### What's the purpose of version control?

Version control is used to maintain a history of every change made to a code base. This is useful for a few reasons:
  1. Auditability - you know who has made a change to the system
  2. Visibility - you can see what has recently changed if something's no longer working
  3. Rollback - you can roll back a bad change, or if you deleted something accidentally you can restore it


### What are the core components of version control?

  1. A repository - this is the 'folder' that all your versioned code goes into
  2. A branch - this is a version of the code in a repository (all repos will have a *main* branch - older repos will have a *master* branch)
  3. A commit - this is a set of file changes with a description of what has changed


### What is Subversion and Git?

Subversion was the earlier form of version control. It has a single repository that sits on a server and commits get pushed to a branch on that server. You must be connected to the server to commit changes to your files.

Git is slightly different. You *clone* a repository onto your computer and now you have a complete copy of repository on your local computer. You then commit changes to the *local* repository, then push those changes up to the server.

Git is much more commonplace these days due to its flexibility and the fact that you don't have to be connected to a server to commit changes. You can commit file changes locally all day, then push the changes to the server when appropriate.


## Git
Time to get into the fun stuff

### Phrases
This is Git specific. Here's a bunch of phrases to help you get familiar with the lingo:
  1. *I cloned the repo*  
     I took a copy of the repository on the server and downloaded it to my local computer  
     `git clone my-repo-name`
  2. *I checked out the 'main' branch*  
     I currently have, sitting in the repository folder, the version of the code that is on the branch named 'main'  
     `git checkout main`
  3. *I just committed the files*  
     I made a series of changes to some files, then batched those changes together and gave the changes a description. The change was committed to the branch that was checked out. 
     ```
     git add .
     git commit -m your-message-here
     ```
  4. *I've pushed those changes*  
     I've pushed the commits on my local branch to the server  
     `git push origin your-branch-name`
 
 ### Exploring things in GitHub
 <details>
  <summary>Task: Find the history for this repository</summary>
    
  #### To show the list of commits with the files that have changed:
  1. On this page, find the green "Code" button near the top
  2. Below this button look for the phrase "XX commits"
  3. Click the XX number
  4. Have a look at the history from the beginning
     You should see a bunch of descriptions. These are the **commits**
  5. Click into a commit by clicking on the **commit message**. Look for the 
     1. Commit message and description
     2. What branch it was committed to
     3. The commit hash (that looks like '57b93de3b28ca38121ab286140a22dedeb2e89a7')
     4. The files that have changed and the changes that were made
</details>
