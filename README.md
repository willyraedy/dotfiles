# Dotfiles

These are my dotfiles. Currently just checking in the files directly in my home directory using the strategy defined here: [https://developer.atlassian.com/blog/2016/02/best-way-to-store-dotfiles-git-bare-repo/](https://developer.atlassian.com/blog/2016/02/best-way-to-store-dotfiles-git-bare-repo/).

## Installation

* Before beginning the steps, make sure computer is updated to the latest operating system

To install on a new machine do:
1. Set up github ssh access (create new key, add to github)

1. Set up the alias for 'dotfiles' in the current shell scope
  `alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'`

1. Clone the repo:
  `git clone --bare <git-repo-url> $HOME/.dotfiles`

1. Make sure you're in the home directory and then checkout the dotfiles
  `dotfiles checkout`


## Other installs to finish setup for computer

1. [https://brew.sh/](homebrew)

1. Homebrew packages (includes casks)
  `brew bundle`

1. [Make default shell zsh](https://support.apple.com/en-ca/HT208050)

1. [Install oh-my-zsh](https://ohmyz.sh/#install)

1. [Install nvm](https://github.com/nvm-sh/nvm#installing-and-updating)
    - Listed on homebrew but unsupported
    - Restart terminal after install

1. Run `nvm install node`

1. [Install Anaconda](https://docs.anaconda.com/anaconda/install/mac-os/) and python through anaconda

## Test Install

1. Run `node` and expect repl to start

1. Run `python` and expect python of version >3 repl to start

1. Test postgres

1. Test mongo
