Yann Lugrin's dotfiles
===================

Requirements
------------

Homebrew installed:

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Git installed:

    brew install git zsh

Set zsh as your login shell:

    chsh -s /bin/zsh

Install
-------

Clone onto your laptop:

    cd ~; git clone https://github.com/zufrieden/dotfiles.git .dotfiles

Install [rcm](https://github.com/thoughtbot/rcm) and others dependencies
like `vim` and more:

    brew bundle .dotfiles/Brewfile

Install:

    rcup -d .dotfiles -x README.md -x LICENSE -x Brewfile -x bin

This will create symlinks for config files in your home directory. The `-x`
options, which exclude the `README.md`, `LICENSE`, and `Brewfile` files plus
`bin` directory, are needed during installation but can be skipped once the
`.rcrc` configuration file is symlinked in.

You can safely run `rcup` multiple times to update:

    rcup

More informations about my config
---------------------------------

Coming soon (or maybe later).

License
-------

MIT (see LICENSE file)

Inspired by thoughtbot dotfiles licensed under MIT with thoughbot copyright:
https://github.com/thoughtbot/dotfiles

