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
- git status : difference between working directory, the staging index and teh repository
- git status -s
- git reset HEAD <file> : to unstage file
- git reset HEAD
- git reset --soft
- git reset --mixed : default
- git reset --hard
- git diff : shows difference between the repository where HEAD is pointed at Vs working directory
- git diff <file>
- git diff --staged : shows difference between the staging index Vs working directory
- git diff --color-words <file> : shows only different words
- git rm <file> : remove uncommitted file. similar to `git add`. use `git commit -m` to commit and remove file from repository.
- git mv <orig_file> <newname_file> : rename file
- git checkout -- <file> : to discard changes in working directory. "--" indicates from current branch only.
- git checkout <SHA-key> -- <file> : revert to that SHA version
- git revert <SHA> : revert and commit
- git revert -n <SHA> : revert and not committed
- git clean -n : test run of `git clean`
- git clean -f : final run of `git clean`





## Notes
- SHA or SHA1 : Secure Hash Algorithm (1) https://en.wikipedia.org/wiki/SHA-1
- toggle between long commits : forward (f) or backward (b). space bar or enter to see more details
- toggle fold long lines : minus sign (-) + shift + S + return. wrap it around instead of lines being truncated.
- to return to long lines (unwrap) : minus sign (-) + S + return
- cat .git/master : points to where HEAD (SHA) is located
- cat .git/refs/heads/master : points to where HEAD (SHA) is located

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
