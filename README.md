# T4SG Git Workshop (F23-S24) Activity

This activity consists of a series of small exercises to apply the concepts in the workshop slides in practice. In the activity, you will:
- add, commit, and commit changes to a forked version of the repository 
- create new branches and practice merging, rebasing, and creating pull requests 
- resolve merge conflicts 
- revert and reset commits 

Aside from forking and cloning the repository on to your machine, all the exercises below can be done independently. Feel free skip questions if you're stuck or want to move on! 

#### Exercise 1: Fork and Clone the Repository
Creating a fork of a repository is analagous to creating a copy of google slide or doc. A fork serves as another remote repository that is independent from the original. Typically, a change in one repository won't affect the other, though to sync a fork with it's parent.  

To create, a fork, in the ***Code*** of the repository, navigate to the ***Fork*** button in the right-hand corner. From there, you'll be prompted to select an owner of the fork (i.e. your account), a name, and a description. After filling in the fields, 
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
