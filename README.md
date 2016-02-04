# Git-Essential-Training

## Commands
- which git
- git --version
- vi /etc/gitconfig
- vi ~/.gitconfig : user level git config file
- vi [PROJECT_PATH]/.git/config : project level git config file
- git config --system : system level configuration
- git config --global : user level configuration
- git config : project level configuration
- git config --global user.name "[NAME]"
- git config --list : list of config properties
- git config --global core.excludefile ~/.gitignore_global : global config for gitignore
- git --help
- git init : initialize repository
- ls -la .git : shows git config files
- git add . : add all uncommitted changes from project. dot (.) is current directory
- git commit -m "message" : commit changes with message
- git commit -am "message" : shorthand for `git add .` and `git commit -m "message"` (grabs everything. not tracked(new) and deleted files are not included)
- git commit --amend -m "message" : this command is a convenient way to fix up the most recent commit.
- git log : check git commit log
- git log -2 : restrict show commit log to last two
- git log --since=2016-01-12 : show commits after this date
- git log --until=2016-01-12 : show commits till this date
- git log --author="Kaustubh" : show commits for specified author
- git log --grep="st" : show commits having specified text
- git log --online : shows all logs in one line
- git log --online -[number] : restrict log for given number
- git log [SHA]..[SHA] : shows log between two mentioned commits
- git log [file] : shows details about file
- git log -p : more details about commit. Like code insertion etc
- git log --stat --summary
- git log --format=oneline : this is similar to `git log --oneline"
- git log --format=[oneline / short / medium / fuller / email / raw]
- git log --graph
- git log --oneline --graph --all --decorate
- git status : difference between working directory, the staging index and teh repository
- git status -s
- git reset HEAD [file] : to unstage file
- git reset HEAD
- git reset --soft
- git reset --mixed : default
- git reset --hard
- git diff : shows difference between the repository where HEAD is pointed at Vs working directory
- git diff [file]
- git diff --staged : shows difference between the staging index Vs working directory
- git diff --cached : similar to `git diff --staged`
- git diff --color-words [file] : shows only different words
- git diff [SHA] : difference between working directory and directory at that point of time
- git diff [SHA] [file]
- git diff [SHA]..[SHA] : difference between two commits
- git diff [SHA]..[SHA] [file]
- git diff -b : is same as `git diff --ignore-space-change`
- git diff -w : is same as `git diff --ignore-all-space`
- git diff [branch-1]..[branch-2]
- git diff [branch-1]..[branch-2]^ : compare with previous commit of branch-2
- git rm [file] : remove uncommitted file. similar to `git add`. use `git commit -m` to commit and remove file from repository.
- git rm --cached [file] : remove from caching (or staging index)
- git mv [orig_file] [newname_file] : rename file
- git checkout -- [file] : to discard changes in working directory. "--" indicates from current branch only.
- git checkout [SHA-key] -- [file] : revert to that SHA version
- git revert [SHA] : revert and commit
- git revert -n [SHA] : revert and not committed
- git clean -n : test run of `git clean`
- git clean -f : final run of `git clean`
- git ls-tree HEAD
- git ls-tree [branch-name]
- git ls-tree [branch-name] [folder-path]
- git ls-tree [branch-name]^ [folder-path] : earlier commit
- git ls-tree [SHA]
- git show [SHA]
- git branch : list branch names in working directory
- git branch [branch-name] : creates new branch
- git branch -d [branch-name] : delete branch (before this make sure you are not working on this branch)
- git branch -D [branch-name] : force delete branch
- git branch -m [branch-new-name] : rename branch
- git checkout [branch-name] : change working directory to specified branch name
- git checkout -b [branch-name] : create and checkout at the same time for new branch



## Notes
- SHA or SHA1 : Secure Hash Algorithm (1) https://en.wikipedia.org/wiki/SHA-1
- toggle between long commits : forward (f) or backward (b). space bar or enter to see more details
- toggle fold long lines : minus sign (-) + shift + S + return. wrap it around instead of lines being truncated.
- to return to long lines (unwrap) : minus sign (-) + S + return
- cat .git/master : points to where HEAD (SHA) is located
- cat .git/refs/heads/master : points to where HEAD (SHA) is located
- project/.gitignore : file to specify which files or directory to ignore
- .gitkeep : use this file to track empty folder

## Contents
http://www.lynda.com/Git-tutorials/Git-Essential-Training/100222-2.html

- Introduction
    - Introduction
    - How to use the exercise files

- Welcome
    - What you should know before watching this course
    - Using the exercise files

1. What is Git?
    - Understanding version control
    - The history of Git
    - About distributed version control
    - Who should use Git?

2. Installing Git 
    - Installing Git on a Mac
    - Installing Git on Windows
    - Installing Git on Linux
    - Configuring Git
    - Exploring Git auto-completion
    - Using Git help
    
3. Getting Started
    - Initializing a repository
    - Understanding where Git files are stored
    - Performing your first commit
    - Writing commit messages
    - Viewing the commit log
    
4. Git Concepts and Architecture
    - Exploring the three-trees architecture
    - The Git workflow
    - Using hash values (SHA-1)
    - Working with the HEAD pointer
    
5. Making Changes to Files
    - Adding files
    - Editing files
    - Viewing changes with diff
    - Viewing only staged changes
    - Deleting files
    - Moving and renaming files

6. Using Git with a Real Project
    - Introducing the Explore California web site
    - Initializing Git
    - Editing the support phone number
    - Editing the backpack file name and links
    
7. Undoing Changes
    - Undoing working directory changes
    - Unstaging files
    - Amending commits
    - Retrieving old versions
    - Reverting a commit
    - Using reset to undo commits
    - Demonstrating a soft reset
    - Demonstrating a mixed reset
    - Demonstrating a hard reset
    - Removing untracked files

8. Ignoring Files
    - Using .gitignore files
    - Understanding what to ignore
    - Ignoring files globally
    - Ignoring tracked files
    - Tracking empty directories

9. Navigating the Commit Tree
    - Referencing commits
    - Exploring tree listings
    - Getting more from the commit log
    - Viewing commits
    - Comparing commits

10. Branching
    - Branching overview
    - Viewing and creating branches
    - Switching branches
    - Creating and switching branches
    - Switching branches with uncommitted changes
    - Comparing branches
    - Renaming branches
    - Deleting branches
    - Configuring the command prompt to show the branch

11. Merging Branches
    - Merging code
    - Using fast-forward merge vs. true merge
    - Merging conflicts
    - Resolving merge conflicts
    - Exploring strategies to reduce merge conflicts