# Useful Command Line Aliases

Add lines below to `~/.bashrc` or `~/.zshrc` if using [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh)

```sh
# Basic aliases
alias s="git status"
alias f="git diff"
alias a="git add"
alias ca="git commit -am"
alias c="git commit -m"
alias d="git pull origin"
alias u="git push origin"
alias l="git log --stat"
alias lp="git log -p"
alias o="git checkout"
alias brm="git branch -D"
alias amend="git commit -a --amend"
alias wip="git add -u && git commit -m 'WIP'"
alias undo="git reset HEAD~1 --mixed"

# Branch grooming
# removes all branches that are already merged in master
alias groom="git checkout master;git pull origin master;echo 'Deleting:';git branch --merged;git branch --merged | xargs git branch -d;echo '';echo 'Branches left:';git branch --no-merged"

# Show recent branches
alias recent='git for-each-ref --sort=committerdate refs/heads/ --format='\''%(HEAD) %(color:yellow)%(refname:short)%(color:reset) - %(color:red)%(objectname:short)%(color:reset) - %(contents:subject) - %(authorname) (%(color:green)%(committerdate:relative)%(color:reset))'\'''

# Refresh the terminal
alias src='source ~/.zshrc'

echo "☀️"
```
