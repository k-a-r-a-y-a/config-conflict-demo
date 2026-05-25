# Git Undo Operations: Revert vs Reset

## Exercise Overview
This repository demonstrates three different methods to undo bad commits, specifically simulating a broken configuration deployment to production.

## The Scenario
- **Good deployment**: Working production config (v1.0.0)
- **Bad deployment**: Broken config causing app crashes (v1.0.1-bad)
- **Goal**: Undo the bad deployment and restore working state

## Three Methods Compared

### 1. `git revert` - SAFEST for shared branches
- this method creates a new commit that undoes the changes and preserves the entire history without deletion

### 2 git reset --soft
- this method removes the commit but keeps changes in staging area
- used when you havent pushed changes to remote yet

### 3 git reset --hard
- this method completely removes the commit and discards all changes in working directory
- used when one wants to completely discard changes

