# Introduction

I use [vim-plug](https://github.com/junegunn/vim-plug) to manage my vim plugins.

Currently, the vim plugins are for reading code in C and Rust.

- C: [cscope](http://cscope.sourceforge.net/cscope_vim_tutorial.html)
- Rust: [rust-analyzer](https://rust-analyzer.github.io/manual.html#vimneovim)

# Installation

## Clone and Install this repo

```
$ git clone https://github.com/MrXinWang/my_vim_configuration
$ cd my_vim_configuration
$ cp .vimrc ~/.vimrc  
$ cp -r .vim ~/.vim  
```

## `vim-plug` Installation

```
$ curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Then, run `:PlugUpdate` in vim to update the plugins. After the update is
finished, you can review the changes by pressing D in the window, or you
can do it later by running `:PlugDiff`.

## `cscope` Installation

```
$ sudo apt update 
$ sudo apt install -y cscope
```

The configuration of vim is already contained in `.vimrc`.

## `rust-analyzer` Installation

The `rust-analyzer` is required `node.js` installed.

```
$ sudo curl -sL install-node.now.sh/lts | sudo bash
```

With the `vim-plug` installed, run `:CocInstall coc-rust-analyzer` in vim
to install coc-rust-analyzer.

The configuration of vim is already contained in `.vimrc`.
