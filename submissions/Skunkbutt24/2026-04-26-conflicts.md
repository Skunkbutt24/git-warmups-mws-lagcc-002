# 2026-04-26 - conflicts

## Drill I did
conflicts.md

## What I ran
git checkout Skunkbutt24  
echo "hello from main" > conflict-demo.txt  
git add conflict-demo.txt  
git commit -m "chore: add conflict demo file"  
git checkout -b scratch/conflict-branch  
echo "hello from branch" > conflict-demo.txt  
git add conflict-demo.txt  
git commit -m "chore: change demo text on branch"  
git checkout Skunkbutt24  
echo "hello from home" > conflict-demo.txt  
git add conflict-demo.txt  
git commit -m "chore: change demo text on home branch"  
git merge scratch/conflict-branch  
cat conflict-demo.txt  
echo "hello from home and branch" > conflict-demo.txt  
git add conflict-demo.txt  
git commit -m "fix: resolve merge conflict on conflict-demo.txt"  
git branch -d scratch/conflict-branch  

## What I learned or re-learned
I learned that a merge conflict happens when two branches change the same part of the same file differently. Git cannot automatically decide which version to keep, so it pauses the merge and asks me to fix the file manually.

I also learned that conflict markers show the two competing versions. `HEAD` shows the version from my current branch, and the other section shows the version from the branch I am trying to merge. To finish the conflict, I have to remove the conflict markers, choose the final text, stage the file with `git add`, and commit the resolution.

## What still feels slow
I still need more practice reading conflict markers and understanding which side comes from my current branch versus the branch being merged.