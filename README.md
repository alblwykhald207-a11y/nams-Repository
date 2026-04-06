# Advanced Git Commands Documentation

## 1. git stash
### Description
`git stash` is used when you want to save your uncommitted changes without committing them. This is helpful when you need to switch branches and don’t want to commit half-done work.

### Example
```bash
// Save your uncommitted changes
git stash

// Switch to another branch
git checkout other-branch

// Apply your stashed changes
 git stash apply
```

## 2. git cherry-pick
### Description
`git cherry-pick` allows you to apply the changes introduced by specific commits from one branch onto another branch.

### Example
```bash
// Switch to the target branch
git checkout target-branch

// Cherry-pick a specific commit
 git cherry-pick <commit-hash>
```

## 3. git revert
### Description
`git revert` is used to create a new commit that undoes the changes made by a specific commit. Unlike `git reset`, which removes commits, `git revert` keeps the history intact.

### Example
```bash
// Revert a specific commit
 git revert <commit-hash>
```

## 4. git reset
### Description
`git reset` can be used to remove commits from the history or to unstage changes. It can be used in three modes: soft, mixed, and hard.

### Use Cases
- **Soft Reset:** Unstages changes but keeps them in the working directory.
- **Mixed Reset:** Resets the index but not the working directory.
- **Hard Reset:** Resets both the index and working directory.

### Example
```bash
// Soft reset to a previous commit
git reset --soft <commit-hash>
// Mixed reset
git reset --mixed <commit-hash>
// Hard reset
git reset --hard <commit-hash>
```

## Conclusion
These advanced Git commands are essential for managing your code effectively. Use them wisely to handle branches, commits, and changes in a more controlled manner.