# Zsh

## Install and Plugin Manager

* [Oh My ZSH!](https://ohmyz.sh/)
  * [github](https://github.com/robbyrussell/oh-my-zsh)

## Plugin

* git
* sudo
* history
* taskwarrior
* tmux
* tmuxinator
* zsh-completions
* zsh-highlighting
* zsh-autosuggestions
* [vi-mode](#Use-oh-my-zsh-plugin)
* vscode
* web-search - Adds several commands to do web search.

## Turn on VIM Mode

### The built-in VIM mode in shell

In Zsh

```zshrc
bindkey -v
```

> In Bash
>
> ```bashrc
> set -o vi
> ```

* Ctrl+R search (fixed by using the oh-my-zsh plugin)

    > The default zsh vim mode will disable the default keybind like Ctrl+R search.
    > (And will not show the current mode is insert mode (`[I]`) or normal mode (`[N]`) so not recommand.)
    > Just add the following line to `~/.zshrc` to map it back.
    > (The `fzf` plugin will be override if you put the vi-mode setting before `[ -f ~/.fzf.zsh ] && source ~/.fzf.zsh`. So be careful)
    >
    > ```zshrc
    > # allow v to edit the command line (standard behaviour)
    > autoload -Uz edit-command-line
    > bindkey -M vicmd 'v' edit-command-line
    >
    > # allow ctrl-p, ctrl-n for navigate history (standard behaviour)
    > bindkey '^P' up-history
    > bindkey '^N' down-history
    >
    > # allow ctrl-h, ctrl-w, ctrl-? for char and word deletion (standard behaviour)
    > bindkey '^?' backward-delete-char
    > bindkey '^h' backward-delete-char
    > bindkey '^w' backward-kill-word
    >
    > # allow ctrl-r and ctrl-s to search the history
    > bindkey '^r' history-incremental-search-backward
    > bindkey '^s' history-incremental-search-forward
    >
    > # allow ctrl-a and ctrl-e to move to beginning/end of line
    > bindkey '^a' beginning-of-line
    > bindkey '^e' end-of-line
    > ```

* `ci"` Functionality: add the following line in `~/.zshrc`

    ```zshrc
    autoload -U select-bracketed
    autoload -U select-quoted
    zle -N select-quoted
    zle -N select-bracketed
    for km in visual viopp; do
        bindkey -M $km -- '-' vi-up-line-or-history
        for c in {a,i}${(s..)^:-\'\"\`\|,./:;-=+@}; do
            bindkey -M $km $c select-quoted
        done
        for c in {a,i}${(s..)^:-'()[]{}<>bB'}; do
            bindkey -M $km $c select-bracketed
        done
    done
    ```

### Use oh-my-zsh plugin

* [oh-my-zsh/plugins/vi-mode](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/vi-mode)
  * [plugins/vi-mode/vi-mode.plugin.zsh](https://github.com/robbyrussell/oh-my-zsh/blob/master/plugins/vi-mode/vi-mode.plugin.zsh)
  * [`ctrl-r` stopped working after enabling `vi-mode` #5213](https://github.com/robbyrussell/oh-my-zsh/issues/5213)
  * ["^r" search not working #635](https://github.com/robbyrussell/oh-my-zsh/issues/635)
  * [Please, add support of " " and ' ' text objects to vi-mode plugin #5708](https://github.com/robbyrussell/oh-my-zsh/issues/5708)

Just add the `vi-mode` in the list of `plugins` like

```zshrc
plugins=(... vi-mode)
```

And this is already include the "keybinding step" that I listed above. So it's ready to go!

### Others

* [softmoth/zsh-vim-mode](https://github.com/softmoth/zsh-vim-mode)
* [Better Vi Mode in Zshell](http://stratus3d.com/blog/2017/10/26/better-vi-mode-in-zshell/)
* [How do I perform a reverse history search in ZSH's vi-mode?](https://unix.stackexchange.com/questions/44115/how-do-i-perform-a-reverse-history-search-in-zshs-vi-mode)

## Optimize Startup Time

* [**Faster and enjoyable ZSH (maybe)**](https://htr3n.github.io/2018/07/faster-zsh/)
* [Speeding up my ZSH load](https://carlosbecker.com/posts/speeding-up-zsh/)
* [How to profile your zsh startup time](https://esham.io/2018/02/zsh-profiling)
