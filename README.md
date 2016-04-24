# Useful Command Line Aliases

Add lines below to `~/.bashrc` or `~/.zshrc` if using [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh)

```
echo "Welcome!"

# Git aliases

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

# Branch grooming
# removes all branches that are already merged in master

alias groom="git checkout master;git pull origin master;echo 'Deleting:';git branch --merged;git branch --merged | xargs git branch -d;echo '';echo 'Branches left:';git branch --no-merged"

# Making docker default machine work, if developing with Docker
# eval "$(docker-machine env default)"

# Extending file system resources to unlock Grunt webfont task when a lot of files are handled.
# ulimit -n 4096

# Go exports, if working on a Go app
# export GOPATH=~/[path to current go project workspace directory]
# export PATH="$PATH:/usr/local/go/bin:$GOPATH/bin"

echo "Have a wonderful day :)"
```