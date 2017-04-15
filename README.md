# My Dotfiles

These are my personal configuration files, and are meant to extend [thoughtbot's
dotfiles][1].  I keep my personal dotfiles isolated to avoid overwriting them
when I update thoughtbot's dotfiles on my machine. My dotfiles include:

* tmux config
* zshell config
* vim config
* vim plugins (via bundles)

[1]: https://github.com/thoughtbot/dotfiles/

## Example of how `.local` dotfiles work

The standard configuration for **vim** is installed at
`~/.vimrc`. thoughtbot dotfile's will overwrite this config file.
thoughtbot's dotfiles include `source ~/.vimrc.local` at the end of
the config so it sources your local dotfiles.

## Installation

```
$ git clone https://github.com/jasonramirez/dotfiles_local.git
```

From the `ditfiles_local` directory, symlink any `*.local` dotfiles:

```
$ ./setup.sh
```

#### Manual Symbolic linking

OSX:

```
$ ln /Users/username/dotfiles_local/.vimrc.local ~/.vimrc.local
```

## Files

* [.tmux.conf.local](https://github.com/jasonramirez/dotfiles_local/blob/master/.tmux.conf.local)
* [.vimrc.bundles.local](https://github.com/jasonramirez/dotfiles_local/blob/master/.vimrc.bundles.local)
* [.vimrc.local](https://github.com/jasonramirez/dotfiles_local/blob/master/.vimrc.local)
* [.zshrc.local](https://github.com/jasonramirez/dotfiles_local/blob/master/.zshrc.local)
