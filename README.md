# Ellie's Linux Dotfiles
!!! This is outdated, I will updated once I get a chance !!!
## What is this?
These are my personal configuration files I use on my Fedora Linux machines.
## What is the structure here?
These configuration files are installed locally using GNU Stow, and are organized in a format Stow understands.  Each directory in this repo is a package, and each sub-directory corrisponds to the location Stow "installs" the package. (Creates a symlink to the package at that location)  Package names typically corrispond to the application to which they relate to.  
For example, `./sway/` belongs to the Stow package `sway`, where the file `./sway/dot-config/sway/config` would be symlinked to `~/.config/sway/config` when installed.  
## How do I test this out?
- Install Fedora Linux
  - Other linux distubtions will probrably work, but will likely require modification.
- Install GNU stow. `sudo dnf install stow` on Fedora.
- Install applications needed.
  - See the list below for all applications which have config files!
- Clone this repo (I use `~/Dotfiles/`)
- Run `stow --dotfiles */` to install all config files, or `stow --dotfiles [Package Name]` to install a specific package.
  - This will create symlinks from
  - The `--dotfiles` option translates files beginning with `dot-*` to `.*` which allows for easier editing.
- Edit by editing the files in the git directory, and Stow-ing again whenever new files are added.
## Applications
- **Bash** shell
- **Foot** Terminal Emulator
- **GTK 3** for applications that use GTK 3.
- **Hyfetch** Neofetch, but with pride flags!
- **Neovim** is better than emacs!
  - Located in `./nvim/`
- **Sway WM**, I3WM, but with Wayland
- **Waybar** status bar for Sway WM
- **ZSH** The shell I actually use!
