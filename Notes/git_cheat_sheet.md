# Cheat Sheet

## Git Checkout
To discard changes that has not yet been committed you write:

`git checkout .`

to discard everything, or:

`git checkout <filename>`

to discard individual files.

## Git Reset
When you have a commit and would like to discard it you write:

`git reset --hard HEAD~2`

This will move your HEAD pointer back two commits and delete everything _above_ the moved HEAD pointer.

If you would like to preserve the commits you'd do:

`git reset --soft HEAD~2`

### Example
You would like to move the last two commits to a new branch

```
git checkout -b new_branch_name_here

git reset --hard HEAD~2
```

To go to the branch afterwards you'd do:

`git checkout new_branch_name_here`
