# Awesome Tools in Linux

## bat
https://github.com/sharkdp/bat

`batcat` syntax highlighting version `cat`

## fzf
https://github.com/junegunn/fzf

```
sudo apt install fzf
```
Edit `~/.bashrc`

```bash
alias fzf="fzf --preview 'batcat --color=always --style=numbers --line-range=:500 {}'"
```
### Move
`Ctrl + j`
`Ctrl + k`
