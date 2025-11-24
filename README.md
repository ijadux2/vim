# Vim Configuration

This repository contains a comprehensive Vim configuration with modern plugins and settings for an efficient development experience.

## Features

### Plugin Management
Uses [vim-plug](https://github.com/junegunn/vim-plug) for plugin management with the following plugins:

- **UI & Appearance**
  - `catppuccin/vim` - Catppuccin color scheme (mocha variant)
  - `vim-airline/vim-airline` - Enhanced status line
  - `vim-airline/vim-airline-themes` - Airline themes
  - `ryanoasis/vim-devicons` - File type icons
  - `preservim/nerdtree` - File explorer
  - `tiagofumo/vim-nerdtree-syntax-highlight` - Syntax highlighting for NERDTree

- **Git Integration**
  - `tpope/vim-fugitive` - Git commands
  - `airblade/vim-gitgutter` - Git diff indicators
  - `Xuyuanp/nerdtree-git-plugin` - Git status in NERDTree

- **Editing & Productivity**
  - `tpope/vim-surround` - Surround text objects
  - `tpope/vim-commentary` - Comment/uncomment functionality
  - `junegunn/fzf.vim` - Fuzzy finder
  - `ctrlpvim/ctrlp.vim` - File finder
  - `WolfgangMehner/bash-support` - Bash script support

- **Language Support**
  - `prabirshrestha/vim-lsp` - LSP client
  - `mattn/vim-lsp-settings` - LSP server configurations
  - `prabirshrestha/asyncomplete.vim` - Async completion
  - `prabirshrestha/asyncomplete-lsp.vim` - LSP completion integration
  - `neoclide/coc.nvim` - Concurrency of completion
  - `ziglang/zig.vim` - Zig language support

## Configuration

### Basic Settings
- **Indentation**: 2 spaces, smart tabs, C-style indentation
- **Appearance**: True colors, dark background, line numbers (relative and absolute)
- **UI**: Enhanced status line, cursor line highlighting, mouse support
- **Font**: JetBrains Mono Nerd Font (12pt)

### Key Mappings

#### File Navigation
- `Ctrl+n` - Toggle NERDTree file explorer

#### LSP Features
- `gd` - Go to definition
- `gr` - Go to references  
- `K` - Hover documentation
- `<leader>rn` - Rename symbol
- `<leader>ca` - Code actions

#### Completion
- `Tab`/`Shift+Tab` - Navigate completion menu
- `Enter` - Accept completion
- `Ctrl+Space` - Force refresh completion

### Customization
- **NERDTree**: Shows hidden files by default
- **Airline**: Powerline fonts enabled, Catppuccin theme
- **Devicons**: Conceals filenames for cleaner display
- **LSP**: Auto-completion with 200ms delay

## Installation

1. Install [vim-plug](https://github.com/junegunn/vim-plug):
   ```bash
   curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
     https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
   ```

2. Copy `.vimrc` to `~/.vimrc`

3. Install plugins:
   ```bash
   vim +PlugInstall +qall
   ```

4. Install required fonts (JetBrains Mono Nerd Font) for proper icon display

## Requirements
- Vim 8.0+ with `+termguicolors` support
- JetBrains Mono Nerd Font (or similar Nerd Font)
- Git (for some plugins)