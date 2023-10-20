
# 🌠 Git Notes for ME!

## Re-writing a Pushed Commit
In Turkish, there's a saying "aman dilemek", which means to plead or beg for something.  
Just like we might beg for forgiveness for a mistake, in Git, we "amend" our last bad commit messages to make them right.  
Modify the last commit's message:

```bash
git commit --amend -m "New commit msg"
```
then force push :
```bash
git push origin <branch-name> --force
```

## Rolling Back Unstaged Changes
Sometimes, curiosity gets the better of us and we tinker with files, only to realize it's not the change we wanted.   
Ever felt like you've opened Pandora's box with a file and wished for a quick escape?   
Especially with those pesky UI files where manual reversion feels like the stone age.
Before you've added, committed, or pushed, there's a magic spell to revert your file back to its last committed state:

```bash
git checkout -- <filename>
```
## Stashing and Dropping: A Clean Slate
Ever been in the middle of some code alchemy and needed to switch gears without committing?   
Enter git stash - your workspace's magic cloak. It hides your changes, letting you pivot swiftly.
```bash
git stash
```
But what if you decide those stashed changes were just a wild experiment not worthy of the light of day?  
No worries. With git stash drop, you can discard that stash, no strings attached.
```bash
git stash drop
```
