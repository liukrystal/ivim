# ivim - An easy & highly customizable vim configuration 

```
    _       _          
   (_)   __(_)___ ___  
  / / | / / / __ `__ \ 
 / /| |/ / / / / / / / 
/_/ |___/_/_/ /_/ /_/  
```

**Version: 2.5**

**Note: From v2.5, ivim uses [vim-plug](https://github.com/junegunn/vim-plug) instead of [NeoBundle](https://github.com/Shougo/neobundle.vim) to manage vim plugins. Please see [vim-plug docs](https://github.com/junegunn/vim-plug) to see the usage.**

**New: You could install the minimum ivim now for fast and basic usage!!!**

> ivim mini only supports terminal vim, and speeds up startup time through loading
> fewer plugins.
>
> Install:
>
> `bash <(curl -L https://raw.githubusercontent.com/kepbod/ivim/master/setup.sh) -m`
>
> or
>
> `bash <(wget --no-check-certificate https://raw.githubusercontent.com/kepbod/ivim/master/setup.sh -O -) -m`
>
> See more information from https://github.com/kepbod/ivim/blob/master/vimrc_mini

*Some new features will be firstly tested in vimrc_mini*

## Features

***Beautiful***

Use lots of famous colorschemes to make your eyes feel comfortable in both Vim and MacVim/gVim.

 * [Hybrid](https://github.com/w0ng/vim-hybrid) (default)

![snapshot1](https://raw.githubusercontent.com/kepbod/ivim/master/snapshot1.jpg)

 * [Gruvbox](https://github.com/morhetz/gruvbox)

![snapshot2](https://raw.githubusercontent.com/kepbod/ivim/master/snapshot2.jpg)

 * [Tender](https://github.com/jacoborus/tender.vim)

![snapshot1](https://raw.githubusercontent.com/kepbod/ivim/master/snapshot3.jpg)

**You could install the patched font from [vim-devicons](https://github.com/ryanoasis/vim-devicons).**

***Efficient***

 * Make using Vim more convenient and faster, and lots of useful plugins confirm a better performance of Vim.

 * To view the full plugin list, please refer [here](https://github.com/kepbod/ivim/blob/master/vimrc#L140).

## Requirements

**Vim**

 * This distribution is adapted to both [Vim](http://www.vim.org/download.php) and [MacVim](http://www.vim.org/download.php#mac)/[gVim](http://www.vim.org/download.php#pc). Remember that the Vim/MacVim/gVim version should be 7.3+, or errors would occur!

**Git**

 * All the installations are based on [Git](http://git-scm.com/) which is a famous distributed revision control system. If you use Windows, you may need install [msysgit](http://msysgit.github.com//).

**Ctags**

 * Ctags generates an index (or tag) file of language objects found in source files that allows these items to be quickly and easily located by a text editor or other utility. I recommend you to use [Exuberant Ctags](http://ctags.sourceforge.net/).

*To use this distribution with less bugs, please get more suggestions from [here](https://github.com/kepbod/ivim/wiki/Tips-for-ivim).*

## Installation

### Manual Installation

0. A Vim/MacVim/gVim with version higher than 7.3 should be installed on your computer;
1. Get ivim from github website, `git clone git://github.com/kepbod/ivim.git $HOME/.ivim`;
2. Make symbolic links of vimrc to your home directory, `ln -s $HOME/.ivim/vimrc $HOME/.vimrc`;
3. Install vim-plug to install and update plugins, `curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim`;
4. Install plugins, `vim +PlugUpdate +qal`;
5. Just enjoy it!

### Automatic Installation (*nix only)

**via 'curl'**

```bash
bash <(curl -L https://raw.githubusercontent.com/kepbod/ivim/master/setup.sh) -i
```

**via 'wget'**

```bash
bash <(wget --no-check-certificate https://raw.githubusercontent.com/kepbod/ivim/master/setup.sh -O -) -i
```

## Updating

```bash
bash $HOME/ivim/setup.sh -n
```

## Configuration

There are some options you could set through `.vimrc` to configure ivim:
* g:ivim_user -- your username
* g:ivim_email -- your email
* g:ivim_github -- your github
* g:ivim_default_scheme -- color settings (hybrid, gruvbox or tender)
* g:ivim_fancy_font -- using fancy font or not
* g:ivim_show_number -- showing number or not
* g:ivim_autocomplete -- autocomplete engine (NEO: neocomplete/neocomplcache/neosnippet, YCM: YouCompleteMe/UltiSnips)
* g:ivim_bundle_groups -- plugin groups ('ui', 'enhance', 'move', 'navigate', 'complete', 'compile', 'git', 'language')

### Note

* This distribution is completely customisable using `~/.vimrc.ivim.local`(only for `vimrc`), `~/.vimrc.local`, `~/.gvimrc.local` and `~/.vimrc.bundles.local`!
* To make full use of auto-completion and syntax checking, please refer [wiki](https://github.com/kepbod/ivim/wiki/Auto-completion-and-syntax-checking).


## Contributation

Welcome to contribute to ivim, see [issue #31](https://github.com/kepbod/ivim/issues/31) for details. Thank you very much for your supporting!

## Vim Tips

*Learning Vim*

* A good learning method of Vim is vimtutor, a 30 minute tutorial that teaches the most basic Vim functionality hands-on.

    To try it, just type `vimtutor` on terminal.

* To practice vim skills, you can enable hard mode, and it will disable the arrow keys, the 'hjkl' keys, the page up/down keys, and a handful of other keys which allow one to rely on character-wise navigation.

    To enable it, just type `:call HardMode()` in normal mode.

* Another way to get familiar with Vim commands and settings is just rely on the strong help system of Vim.

    It's easy and convenient to type `:h` or `:help` in Vim for help of whatever you want to know.

* A beautiful Vim cheat sheet is available [here](http://michael.peopleofhonoronly.com/vim/). If you want one, just click it!

*Key Mappings*

* Because I have set some key mappings for more convenient typing and checking, you may feel inconvenient with them at start. But if you get familiar with them, I'm sure you will love them.

    You can just type `:map` in Vim to see them.

*More Tips*

* [Vim_Tips_Wiki](http://vim.wikia.com/wiki/Vim_Tips_Wiki) is an excellent website, and you can learn much from it.
* [Vimcasts](http://vimcasts.org) publishes free screencasts about Vim. It's useful and interesting! Believe me!

**Hope You Enjoy Vimming!!!**

## License

Copyright (C) 2012-2016 Xiao-Ou Zhang. See the [LICENSE](https://github.com/kepbod/ivim/blob/master/LICENSE.txt) file for license rights and limitations (MIT).
