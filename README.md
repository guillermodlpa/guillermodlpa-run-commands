# Useful Git Config Aliases

To setup, add these to your `.gitconfig`.

```sh
$ cat .gitconfig-aliases >> ~/.gitconfig
```

##### Shorter syntax to add new files
```sh
$ git a .
```

##### Apply unstaged changes to the previous commit
```sh
$ git amend
```

##### Put the current branch name in your clipboard (Mac Only, needs `pbcopy`)
```sh
$ git b

# ... CMD+V
```

##### Remove local branches already merged to master (or another branch)
```sh
# Remove local branches merged to master
$ git bclean

# Remove local branches merged to develop
$ git bclean develop
```

##### Shorter syntax to remove a branch
```sh
$ git bd some-branch
```

##### Shorter syntax to git diff with Color
```sh
$ git d
$ git d some-branch
$ git d HEAD~1
```

##### Search remote branch names
```sh
$ git find ma

# origin/HEAD -> origin/master
# origin/master
```

##### Shorter syntax to prune remote branches
```sh
$ git grp
```

##### Log with lines of change
```sh
$ git l
```

##### Log with list of files changed
```sh
$ git ll
```

##### Log history for a specific file
```sh
$ git logfile ./somefile.js
```

##### Log with diff of files changed
```sh
$ git lp
```

##### Log with color, condensed
```sh
$ git ls
```

##### Shorter syntax to checkOUT or "open"
```sh
$ git o some-branch
```

##### Shorter syntax to checkout previous branch
```sh
$ git checkout master
$ git checkout some-branch
$ git p
```

##### Push to remote origin
```sh
$ git pb
```

##### Safer Force Push after rebase (prevents overwriting others)
```$
$ git pf
```

##### Show recent branches
```sh
$ git recent
```

##### Shorter syntax for status
```sh
$ git s
```

##### Undo previous commit leaving changes unstaged locally
```sh
$ git undo
```

##### Better `git pull`
```sh
$ git up
```

##### Commit all unstaged changes and new files to "work-in-progress" commit. Works great with `git amend` and `git undo`
```$
$ git wip
```
