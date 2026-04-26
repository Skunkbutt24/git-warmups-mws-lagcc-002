# 2026-04-26-03 - branching

## Drill I did
branching.md

## What I ran
git branch --show-current  
git checkout -b scratch/drill-test  
git branch  
git checkout Skunkbutt24  
git branch -d scratch/drill-test  
git branch  

## What I learned or re-learned
I learned that `git checkout -b` creates a new branch and switches to it at the same time. Without `-b`, `git checkout` only switches to an existing branch. Branches are useful because they let me work on changes separately without affecting the main branch or my personal branch.

I also learned that `git branch` lists local branches, and the branch with the `*` is the branch I am currently using. `git branch -d` deletes a branch safely after I switch away from it.

## What still feels slow
I still need more practice remembering when to use `git checkout -b` to create a branch versus `git checkout` to switch branches.