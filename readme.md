chezmoi-completions for zsh
=============

Chezmoi completions for zsh

## Usage

### Using zsh frameworks

#### [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)

* Clone the repository inside your oh-my-zsh repo:

        git clone https://github.com/jarle/chezmoi-completions ${ZSH_CUSTOM:-${ZSH:-~/.oh-my-zsh}/custom}/plugins/chezmoi-completions

* Add it to `FPATH` in your `.zshrc` by adding the following line before `source "$ZSH/oh-my-zsh.sh"`:

        fpath+=${ZSH_CUSTOM:-${ZSH:-~/.oh-my-zsh}/custom}/plugins/chezmoi-completions/src

Note: adding it as a regular Oh My ZSH! plugin will not work properly.

#### [zplug](https://github.com/zplug/zplug)

Add `zplug jarle/chezmoi-completion` to your `~/.zshrc`.


#### [antigen](https://github.com/zsh-users/antigen)

Add `antigen bundle jarle/chezmoi-completion` to your `~/.zshrc`.


#### [zinit](https://github.com/zdharma-continuum/zinit)

Add `zinit light jarle/chezmoi-completions` to your `~/.zshrc`.

### Manual installation

* Clone the repository:

        git clone https://github.com/jarle/chezmoi-completions.git

* Include the directory in your `$fpath`, for example by adding in `~/.zshrc`:

        fpath=(path/to/chezmoi-completions/src $fpath)

* You may have to force rebuild `zcompdump`:

        rm -f ~/.zcompdump; compinit

### Contributing

Contributions are welcome, see [CONTRIBUTING](https://github.com/jarle/chezmoi-completions/blob/master/CONTRIBUTING.md).


## License
Completions use the Zsh license, unless explicitly mentioned in the file header.
See [LICENSE](https://github.com/jarle/chezmoi-completions/blob/master/LICENSE) for more information.
