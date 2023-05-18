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
export FZF_DEFAULT_OPTS='--height 80% --layout=reverse --border'
export fzf_preview_cmd='[[ $(file --mime {}) =~ binary ]] && echo {} is a binary file || (batcat --color=always {} || highlight -O ansi -l {} || cat {}) 2> /dev/null | head -500' 
```
### Using the finder
`CTRL-K` / `CTRL-J` (or `CTRL-P` / `CTRL-N`) to move cursor up and down
Enter key to select the item, 

`CTRL-C` / `CTRL-G` / `ESC` to exit
On multi-select mode (`-m`), `TAB` and `Shift-TAB` to mark multiple items
Mouse: scroll, click, double-click; shift-click and shift-scroll on multi-select mode
