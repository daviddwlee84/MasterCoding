# VIM Advanced Guide

## Tabs, Windows and Buffers

> **Tabs** for **window container**
>
> **Windows** for **buffer viewports**
>
> **Buffers** for **file proxies** (and the arglist)

Only tab command work in VSCode Vim

### Buffer - file proxy

```vim
:help buffers
```

| Actions         | Description                   |
| --------------- | ----------------------------- |
| `:bn`           | go to next buffer             |
| `:b {filename}` | go to buffer {filename}       |
| `:bd`           | delete current buffer         |
| `:buffers`      | print out all buffers         |
| `:bufdo {cmd}`  | execute {cmd} for all buffers |

#### Arglist

> Can be considered as a subset of the beffer

| Actions            | Description                         |
| ------------------ | ----------------------------------- |
| `:n`               | go to next file (based on arg list) |
| `:arga {filename}` | add {filename} to arg list          |
| `:argl {files}`    | make a local arg copy via {files}   |
| `:args`            | print out all arguments             |

### Window - buffer viewport

```vim
:help windows
```

| Actions        | Description                      |
| -------------- | -------------------------------- |
| `<Ctrl-w> s`   | split window                     |
| `<Ctrl-w> v`   | split window vertically          |
| `<Ctrl-w> o`   | make the window the only one     |
| `<Ctrl-w> q`   | close window                     |
| `<Ctrl-w> w`   | alternate window                 |
| `<Ctrl-w> r`   | rotate window                    |
| `:windo {cmd}` | execute {cmd} for all windows    |
| `:sf {file}`   | split window and `:find {file}`  |
| `vert {cmd}`   | make any split {cmd} be vertical |

#### Window Split and Open File

* [Vim Splits - Move Faster and More Naturally](https://thoughtbot.com/blog/vim-splits-move-faster-and-more-naturally)
* [Switch between Vim window splits easily](https://vim.fandom.com/wiki/Switch_between_Vim_window_splits_easily)

| Actions          | Description                       |
| ---------------- | --------------------------------- |
| `:e {filename}`  | edit {filename} in current window |
| `:sp {filename}` | open {filename} in split window   |

### Tab - window container

```vim
:help tabs
```

| Actions | Description          |
| ------- | -------------------- |
| `gt`    | go to next tab       |
| `gT`    | go to previous tab   |
| `:tabc` | close tab            |
| `:tabe` | open tab             |
| `:tabo` | close all other tabs |

## Mark

> * [Vim Tips Wiki - Using marks](https://vim.fandom.com/wiki/Using_marks)

## Register

## Record Macro

`qq` do some shit `esc`

TODO

## Folding

> * [Vim Tips Wiki - Folding](https://vim.fandom.com/wiki/Folding)

## Other Notes

### Back to Directory

If I open vim in a folder like `vim .`

And I go into a file

I want to get back to the directory mode
[Go to back directory browsing after opening file in vim - Stack Overflow](https://stackoverflow.com/questions/9160499/go-to-back-directory-browsing-after-opening-file-in-vim)
`:b#`

repeat last colon command
[Repeat last colon command | Vim Tips Wiki | FANDOM powered by Wikia](https://vim.fandom.com/wiki/Repeat_last_colon_command)
`@:`

`-`: upper dir

## Resources

### Tutorial

* [**Openwest 2015 - Erik Falor - "From Vim Muggle to Wizard in 10 Easy Steps"**](https://youtu.be/MquaityA1SM)
  * [**Vim_Wizard Slides**](http://unnovative.net/Erik_Falor_Vim_Wizard.pdf)
  * [reddit](https://www.reddit.com/r/vim/comments/3ctlwu/openwest_2015_erik_falor_from_vim_muggle_to/)
  * Erik Falor
    * [personal website](http://unnovative.net/)
    * [github](https://github.com/fadein)
* [**Improving Vim Speed**](https://youtu.be/OnUiHLYZgaA)
* [Ben Orenstein - Write code faster: expert-level vim (Railsberry 2012)](https://youtu.be/SkdrYWhh-8s)
* [YouTube Playlist - Vim screencasts](https://www.youtube.com/playlist?list=PLwJS-G75vM7kFO-yUkyNphxSIdbi_1NKX)
