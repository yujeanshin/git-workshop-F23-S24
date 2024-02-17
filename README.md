# T4SG Git Workshop (F23-S24) Activity

This activity consists of a series of small exercises to apply the concepts in the workshop slides in practice. In the activity, you will:
- add, commit, and commit changes to a forked version of the repository 
- create new branches and practice merging, rebasing, and creating pull requests 
- resolve merge conflicts 
- revert and reset commits 

Aside from forking and cloning the repository on to your machine, all the exercises below can be done independently. Feel free skip questions if you're stuck or want to move on! 

#### Exercise 1: Fork and Clone the Repository
Creating a fork of a repository is analagous to creating a copy of google slide or doc. A fork serves as another remote repository that is independent from the original. Typically, a change in one repository won't affect the other, though to sync a fork with it's parent.  

To create, a fork, in the ***Code*** of the repository, navigate to the ***Fork*** button in the right-hand corner. From there, you'll be prompted to select an owner of the fork (i.e. your account), a name, and a description. 

***Uncheck*** the option to copy the main branch only. For the exercises below, you'll want access to all the branches from the original. 

After filling in the fields, 
click ***Create Fork*** to be re-directed to the new repository. 

Now, to clone the repository, click on ***Code***, and copy the url under HTTPS or 
SSH. From there, in your terminal, run 
```
git clone <git@github.com:USER-NAME/REPOSITORY-NAME.git>

# e.g cloning the original repository
git clone git@github.com:hcs-t4sg/git-workshop-F23-S24.git 
``` 

After cloning, open the repo in you preferred code editor (i.e. VS Code), and in your terminal, enter the directory
```
# list files in current directory
ls 

cd <repo_name> 

# e.g. 
cd git-workshop-F23-S24
```

#### Exercise 2: Create a Branch and Add a Feature
Create a new branch called *answers* and switch to it. 

Create a new file called `answers.md`, and take 3-5 minutes to answer the following
questions: 
1. What is the difference between git and GitHub?
2. Why is version control important?
3. What is the command to view a branch's commit history? 
4. What command lists all the branches in your local repository? Which one lists those in the remote? 
5. To prevent specific files and folders from being commited to a repository, what should you do?

Write your answers in `answers.md` (the format is up to you). After you're finished, 
make a commit and push your changes. Then, make a PR to merge into main. 

Before merging the PR into main, navigate to the ***Files Changed*** tab, where you'll see files with lines highlighted in 
green and red. Looking at the base branch as a baseline, green represents additions in the compare branch while red represents deletions. 

Hover over a line of code and click the plus symbol. Add a sample comment. In PRs, collaborators can reference specific lines of code by making in-line comments. 

Merge `answers` into main and navigate to the branches view of the repository. You'll see that `answers` is now marked as ***Merged*** and is now safe to delete. 






