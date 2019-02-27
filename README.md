# git-rebase-tutorial

Checkout branch `dev` to see the random commits. A few important commands:

```
git fetch # optional, just in case your local branches are behind
git rebase -i <branch_name>
```
Rebase off of the provided branch name, `-i` means "interactive", which will open up a Vim editor with some eligible commits as well as instructions on what commands are available.

If you are not very familiar with Vim, here are some basics: 
* Press `i` to start editing
* Press `Esc` to stop editing
* Press `j, k, l, h` for navigation (or the arrow keys)
* Press `:` and then enter `wq` and press "Enter" key to save and quit editing

Sometimes, if you've already pushed your branch, and then rebased using some of the commands that modified your commit history, then when you try to push again you may get error complaining that your local branch is behind, if this happens, you can push with the `-f` flag.
