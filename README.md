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
- git log : check git commit log
- git log -2 : restrict show commit log to last two
- git log --since=2016-01-12 : show commits after this date
- git log --until=2016-01-12 : show commits till this date
- git log --author="Kaustubh" : show commits for specified author
- git log --grep="st" : show commits having specified text




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
    
- Conclusion
    - Next steps