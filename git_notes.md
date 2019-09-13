# Git
## Usage
I deleted files but used `rm` instead of `git rm`. How do I untrack the deleted files?
```
git add --update
git commit -m "Untrack deleted files"
```
Cloned a new repo that stores files with LFS but files haven't downloaded. How do I download them?
Check that git lfs is installed and then run
```
git lfs pull
```
inside the repo
