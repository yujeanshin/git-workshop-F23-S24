# T4SG Git Workshop (F23-S24) Activity

This activity consists of a series of small exercises to apply the concepts in the workshop slides in practice. In the activity, you will:

- add, commit, and commit changes to a forked version of the repository
- create new branches and practice merging, rebasing, and creating pull requests
- resolve merge conflicts
- revert and reset commits

Aside from forking and cloning the repository on to your machine, all the exercises below can be done independently. Feel free skip questions if you're stuck or want to move on!

#### Exercise 1: Fork and Clone the Repository

Creating a fork of a repository is analagous to creating a copy of google slide or doc. A fork serves as another remote repository that is independent from the original. Typically, a change in one repository won't affect the other, though to sync a fork with it's parent.

To create, a fork, in the **_Code_** of the repository, navigate to the **_Fork_** button in the right-hand corner. From there, you'll be prompted to select an owner of the fork (i.e. your account), a name, and a description.

**_Uncheck_** the option to copy the main branch only. For the exercises below, you'll want access to all the branches from the original.

After filling in the fields,
click **_Create Fork_** to be re-directed to the new repository.

Now, to clone the repository, click on **_Code_**, and copy the url under HTTPS or
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

Create a new branch called _answers_ and switch to it.

Create a new file called `answers.md`, and take 3-5 minutes to answer the following
questions:

1. What is the difference between git and GitHub?
2. Why is version control important?
3. What is the command to view a branch's commit history?
4. What command lists all the branches in your local repository? Which one lists those in the remote?
5. To prevent specific files and folders from being commited to a repository, what should you do?

Write your answers in `answers.md` (the format is up to you). After you're finished,
make a commit and push your changes. Then, make a PR to merge into main.

Before merging the PR into main, navigate to the **_Files Changed_** tab, where you'll see files with lines highlighted in
green and red. Looking at the base branch as a baseline, green represents additions in the compare branch while red represents deletions.

Hover over a line of code and click the plus symbol. Add a sample comment. In PRs, collaborators can reference specific lines of code by making in-line comments.

Merge `answers` into main and navigate to the branches view of the repository. You'll see that `answers` is now marked as **_Merged_** and is now safe to delete.

#### Exercise 3: Merging Branches and Resolving Conflicts

There are two branches `mergeA` and `mergeB` each with markdown files labeled from 1 to 6.
Make a pull request with `mergeA` as the **_compare_** branch and `mergeB` as the **_base_** branch.
Upon comparing each branch, you will see that an automatic merge fails and that you will have to
manually resolve conflict files.

To resolve the conflicts flagged in the PR, merge `mergeB` into
`mergeA` (i.e. `mergeA` will become the merged version of the two) by either accepting the current change,
the incoming change, or both changes. Then, once you've resolved all conflicts and commited and push the merge
to the repository, complete the PR.

#### Exercise 4: Rebasing Branchings

Now, navigate to `rebaseA` and `rebaseB`. Both of these branches should look familiar,
being identical counterparts to the original versions of `mergeA` and `mergeB`. Like exercise 3,
integrate the changes from both branches such that `rebaseB` is combined into `rebaseA`. However, instead
of a merge, use a **_rebase_**.

#### Exercise 5: Squashing Commits

In the branch `squash`, you will see that the last three commits are fairly similar, each adding information
about a T4SG member named Jayden. Squash these three commits into a single commit titled
"added biography information for Jayden".
