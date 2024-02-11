## Summary
My development environment is Windows 11 + WSL (Ubuntu 20.04). Here are some config files I use to enhance my workflow.

### Config for Neovim
- Install NeoVim as shown [here](https://dev.to/asyncedd/building-neovim-from-source-1794)
- Copy `nvim/` directory from this repo to `~/.config/`
- Open `~/.config/nvim/` directory in neovim
- Run `Lazy` neovim command. The Lazy UI must appear
- Press `Shift + S` to sync (install and update) all plugins
    - Note that [dap](https://github.com/CREESTL/LinuxSpecs/blob/master/nvim/lua/creestl/plugins/dap.lua) debugger requires [codelldb](https://github.com/vadimcn/codelldb) to be installed (or linked) to `usr/bin/codelldb`
- Reload neovim

### Config for Tmux
- Copy `tmux/` directory from this repo to `~/.config/`
- Press `CTRL+B SHIFT+I`
- Reload tmux

### Config for Zsh
- Install zsh: `sudo apt install zsh`
- Install Oh My Zsh: `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- Install [exa](https://github.com/ogham/exa) replacement for `ls`
- Install [ScreenFetch](https://github.com/KittyKatt/screenFetch) to see PC info in terminal
- Install [nala](https://github.com/volitank/nala) wrapper for `apt`
- Install [htop](https://github.com/htop-dev/htop) for system processes management
- Install `powerlevel10k` theme via Oh My Zsh. See [guide](https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#oh-my-zsh)
- Copy `.p10k.zsh` file to `~/` directory
- Copy `.zshrc` file to `~/` directory
- Reload zsh

### Config for Git
- Copy `.gitconfig` file to `~/` directory

### Config for VSCode 
*Keys*  
Some key remaps had to be done in `Settings` rather than in `~/.config/nvim/` as well, because VSCode is 
responsible for keyboard inputs. For example the `jk` remap for quitting to Normal Mode. To import this keymaps:
- Open VSCode
- Press `Ctrl + Shift + P`
- Search for `Open Keyboard Shortcuts`
- On the shortcuts page look for a small "file with arrow" icon in the top right corner. Press on that icon
- The `keybindings.json` file will pop up
- Copy the contents of the `vscode_keybindings.json` file from this repo into the `keybindings.json` file opened in VSCode 

*Sync*  
[Settings Sync](https://code.visualstudio.com/docs/editor/settings-sync) was activated to sync settings on all of my devices.  

