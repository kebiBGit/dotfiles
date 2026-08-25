# My dotfiles :) 

You can try it by: 

```bash
mkdir -p ~/.config/my_backup

mv ~/.config/fastfetch ~/.config/ghostty ~/.config/kitty ~/.config/nvim ~/.config/tmux ~/.p10k.zsh ~/.config/my_backup/

git clone --recurse-submodules https://github.com/kebiBGit/dotfiles.git ~/dotfiles

# Copy configuration from cloned repo to your system
cp -r ~/dotfiles/.config ~/
cp ~/dotfiles/.p10k.zsh ~/
```

> [!NOTE]
> Make sure to clone with `--recurse-submodules` so that submodules (such as Neovim and Ghostty shaders) are fetched properly.
> [Neovim](https://github.com/kebiBGit/neovim.git) & [Ghostty-shaders](https://github.com/0xhckr/ghostty-shaders.git) 

> [!NOTE]
> Needs some dependencies to fully support all tools and plugins <br>
> Install the following dependencies to fully support the dotfiles setup :)

```bash
sudo pacman -Syu --needed neovim tree-sitter-cli gcc unzip kitty ghostty tmux zsh fastfetch  # for arch(-based)
# for fully utilizing my neovim config - tree-sitter-cli, gcc, unzip
# for p10k.zsh - install `zsh & powerlevel10k`
```
