# Welcome to my RCFiles

RCFiles - is a bunch of config files of my Linux / OSX enviorement.
Here you can find some of my conf files for:

* vim
* tmux
* zsh
* bash
* oh-my-zsh

## Setup

This section is divide in 2. One for Linux and other for OSX.

### Linux Install

* First you need to clone this repo using git:

```shell
$ git clone https://github.com/nilo/rcfiles.git ~/rcfiles 
```

* Then:

```shell
$ cd ~/rcfiles
$ sh install.sh
```

That's it! Now you need to do some [post install](###markdown-header-post-install).

### Post install

#### Vim:

* Install [Vundle](http://github.com/gmarik/Vundle.vim)

```shell
$ git clone https://github.com/gmarik/Vundle.vim.git ~/rcfiles/bundle/Vundle.vim
```
* Open vim

```shell
$ vim
```

Inside vim
```vim
:PluginInstall
```

* Install Powerline

You need to install `python powerline` to get Vim Airline caracters working proprelly.
If you are in a Linux system like ArchLinux you need to install the `python-powerline-git` package. 
In Archlinux you can use [aur](http://aur.archlinux.org) repository to install it.

```shell
$ packer -S python-powerline-git
```
obs: I'm using packer to manager aur repository but you can use the manual way.

#### Tmux

If you have problem with tmux colors try to start it with: `tmux -2` to use 256 colors.
