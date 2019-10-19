# Git OnBoarding

Resources for onboarding to MScA Robotics

Git is a version control tool. With it you can track all your changes
in a codebase and know when, who, and why that line of code was put 
there. This makes running and debugging software much easier. It 
also unlocks collaboration between team members.

Github has an excellent [introduction to git guide](https://guides.github.com/introduction/git-handbook/)
that you should read.

## Goals

By the end of this walkthrough you will:
  1. Clone this repository
  2. Commit a change locally
  3. Open a PR for that change
  4. Merge PR
  
### Clone this Repository

Directories in git are called _repositories_. There is a repository for 
each Robotics crew. To create a new repository please contact one of
the [org admins](https://github.com/orgs/MScA-Robotics/teams/owners/members). 

### Commit a change locally

Once you have the repository locally, create a new branch

    git checkout -b branch_name
    
Check that your branch was created and you are now on that branch

    git branch
    
Create a new file in the `git_onboarding` directory. 
Make at least two commits to this file.

    git add -A
    git status
    git commit -m "First commit message"
    ...
    git add -A
    git status
    git commit -m "Second commit message"
    
### Open a PR

Push your local branch to GitHub

    git push -u origin branch_name
    
Go to GitHub and confirm you branch has been pushed with those 
commits. 

Open a PR. Tag me `scottshepard` as a reviewer (and whomever else you'd like).
Make sure to include a good title and description.

### Merge the PR 

Your tagged reviewer should now review your PR. If they ask for changes,
make or discuss them. Code review is the first line of defense against
buggy code. For big changes, the reviewer should download the code
locally (with `git checkout branch_name`) and test it themselves.

Once a reviewer has approved the PR, use the squash-and-merge feature.

### GitFlow Rules

1. Commit early, commit often
2. Commits should be atomic
3. Never commit directly to master 
4. Each feature gets its own branch
5. Approval on PR before merge

## Git Commands

Here is a non-exhastive list of common git commands I use every day.

    git status
    git add file_name
    git add -A
    git commit -m "Some commit message"
    git branch
    git branch -vv
    git checkout branch_name
    git checkout -b new_branch_name
    git pull
    git push
    git push -u origin branch_name
