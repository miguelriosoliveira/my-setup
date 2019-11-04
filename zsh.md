## Import zsh_aliases file

```shell
if [[ -f ~/.zsh_aliases ]]; then
    . ~/.zsh_aliases
fi
```

## Add `syntax highlighting` and `autosuggestions`

```shell
mkdir ~/.zsh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.zsh/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
```

## Add these lines to the end of `.zshrc`

```shell
source ~/.zsh/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh
```
