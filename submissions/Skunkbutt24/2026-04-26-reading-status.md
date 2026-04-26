# 2026-04-26-01 - reading-status

## Drill I did
reading-status.md

## What I ran
git status  
git log --oneline  
git log --oneline -5  
git log --graph --oneline --all  
git diff  

## What I learned or re-learned
I learned that `git status` shows the current condition of my working directory and branch. It tells me whether files are untracked, modified, staged, or already committed. I also learned that `git log --oneline` shows commit history in a short format with the commit hash and commit message.

The graph in `git log --graph --oneline --all` shows how commits and branches connect. I also learned that `git diff` shows changes that are not staged yet. If there are no unstaged changes, `git diff` does not show anything.

## What still feels slow
I still need more practice reading `git log --graph` because the branch lines can look confusing at first.