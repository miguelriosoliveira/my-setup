# Make various commits become one
```bash
git rebase -i -s recursive -X theirs <commit sha1 id | branch name>
```

# Make Sublime Text default text editor
```bash
git config --global core.editor "subl3 -n -w"
```

# Beautiful `git log` for terminal
Add this to `.bashrc`, if not already there
```bash
if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi
```
Add this to `.bash_aliases`
```bash
alias gitlog="git log --all --decorate --oneline --graph"
```
