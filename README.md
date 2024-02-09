# Dotfiles
These are my custom dotfiles. 
## Stow
This dotfile repo is intended to be managed with [GNU stow](https://www.gnu.org/software/stow/). To make the process of setting it up easier, it is recommended that the repo is coloned to the `$HOME` folder. To better understand the functionality of stow, this [article](https://dr563105.github.io/blog/manage-dotfiles-with-gnu-stow/#install-stow) is a great read. The basic commands of stow are the following:

```bash
stow <packagename> # activates symlink
stow -n <packagename> # trial runs or simulates symlink generation. Effective for checking for errors
```
Additional commands for cleanup
```bash
stow -D <packagename> # delete stowed package
stow -R <packagename> # restore package
```

## Nvim
My nvim is based on the [ kickstart.nvim ](https://github.com/nvim-lua/kickstart.nvim) project. I have extended it and it keeps growing according to my needs, still a noob in this field

## Tmux
Prefix has been remap to `C-a`. 
Some other commands to have in mind are the following:

### sessions
```bash
C-a d   #detach from sessions
tmux a  #attach to last session
tmux a -t <sesion>  #attach to session 
tmux ls
```
###  windows
```bash
C-a &   #kill window
C-a c   #create window
C-a [i] #go to window [i]
C-a `,` #rename a window
SHIFT-<arrow>   #move between windows 
```
### panes
```bash
C-a |   #create panel vertically
C-a -   #create panel horizontal
C-a x   #delete current
```
