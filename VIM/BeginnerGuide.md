# VIM Biginner Guide

```$
vimtutor
```

## Concept

### The most basic movement and operation

* (TODO) h, j, k, l stuff
* (TODO) open, save and exit file

### VIM Modes and Switch

| Modes             | Sample triggering keystrokes |
| ----------------- | ---------------------------- |
| Normal Mode       | `Esc`                        |
| Insert Mode       | `i`, `a`, `c`                |
| Visual Mode       | `v`, `V`, `<Ctrl-v>`         |
| Command-line Mode | `:`, `/`                     |

### VIM Key Concept

* Operators (verb)
  * e.g. `c`, `d`, `y`
* Text Objects
  * (adjactive) + (noun) or just (noun)
  * (adjactive)
    * `i`: inside
    * `a`: around
  * (noun)
    * `w`/`W`
* Motions

```txt
[count][operator][text object / motion]
```

### Jump Motion and Jump List / Tag Stack

```vim
:help jump-motions
:help jumplist
```

```vim
:help tag-stack
```

| Function        | Back to Previous Position | Goto Next Position                       |
| --------------- | ------------------------- | ---------------------------------------- |
| Using Tag Stack | `<Ctrl-t>`                | `<Ctrl-]>` Tag under cursor (with Ctags) |
| Using Jump List | `<Ctrl-o>`                | `<Ctrl-i>`                               |

## Navigation

> * [**Youtube - Vim Navigation Commands**](https://youtu.be/Qem8cpbJeYc)

(TODO) oragnize the commands in this video

### Shifting Screen

Move current line to

* Top: `zt`
* Middle: `zz`
* Bottom: `zb`

| Function         | Down       | Up         |
| ---------------- | ---------- | ---------- |
| Scroll one line  | `<Ctrl-e>` | `<Ctrl-y>` |
| Scroll half-page | `<Ctrl-d>` | `<Ctrl-u>` |
| Scroll full-page | `<Ctrl-f>` | `<Ctrl-b>` |

## Finding things

### Find the letter/position in the current line

| Function                         | Forward | Backward |
| -------------------------------- | ------- | -------- |
| **F**ind (on) `letter`           | `f`     | `F`      |
| reach **T**ill (before) `letter` | `t`     | `T`      |
| repeat the previous "Find/Till"  | `;`     | `,`      |

e.g. Replacing all the "_" with "-". Like (`This_is_combined_with_underline`): `f_r-;r -;r-;r-`

### Search things under cursor

| Function            | Forward | Backward |
| ------------------- | ------- | -------- |
| Search current word | `*`     | `#`      |
| Next occurrence     | `n`     | `N`      |

### Search things with keyword

> * [Vim Tips Wiki - Searching](https://vim.fandom.com/wiki/Searching)

| Function           | Forward | Backward |
| ------------------ | ------- | -------- |
| Search the pattern | `/`     | `?`      |

### Search things among files

* Ack plugin
* grep

## Replace things

* `r`

### Search and replace

> * [Vim Tips Wiki - Search and replace](https://vim.fandom.com/wiki/Search_and_replace)

## Undo/Redo/Re-do

* `u`: undo last change
* `<Ctrl+r>`: Redo changes which were undone
* `.`: Re-do last command
  * e.g. If I delete a word using `dw`. I can delete again using just `.`.

## MacOS Related

> To copy and paste from your PRIMARY (on OS X, your clipboard) you use the * register

* Copy to clipboard: `"*yy`
* Paste from clipboard: `"*p`

### iTerm Related

## Resources

* [Vim the editor](https://www.vim.org/)
* [Vim Tips Wiki](https://vim.fandom.com/wiki/Vim_Tips_Wiki)
* [Vim (text editor)](https://en.wikipedia.org/wiki/Vim_(text_editor))
* [reddit r/vim](https://www.reddit.com/r/vim/)
* [Vim Cast](http://vimcasts.org/)

### Tutorial

#### Just VIM

* [**Learning Vim in a Week**](https://youtu.be/_NUO4JEtkDw)

#### With Friends (tmux)

* [**vim + tmux - OMG!Code**](https://youtu.be/5r6yzFEXajQ)
  * [nicknisi/vim-workshop](https://github.com/nicknisi/vim-workshop)
  * [blog](https://nicknisi.com/posts/2015-02-25-vim-tmux/)
  * [slides](https://speakerdeck.com/nicknisi/vim-plus-tmux)
* [**Talk on going mouseless with Vim, Tmux, and Hotkeys**](https://youtu.be/E-ZbrtoSuzw)
* [Turn Vim & Tmux into an IDE like environment](https://youtu.be/YD9aFIvlQYs)

### Interactive Tutorial

* [**VIM Adventures**](https://vim-adventures.com/) - Learning VIM while playing a game
* [OpenVim](https://www.openvim.com/)

### How Vim Can Do

* [**Vim notetaking tips**](https://youtu.be/wh_WGWii7UE)
  * [speaker github](https://github.com/connermcd)
* [Integrating Vim Into Your Life](https://thoughtbot.com/blog/integrating-vim-into-your-life)
* [How vim Makes my Daily Life Easier](https://youtu.be/NzD2UdQl5Gc)
* [Vim Makes Everything Better, Especially Your File Manager And Shell!](https://youtu.be/a4scYdubKbo)

### Book

* O'Reilly Learning the vi and Vim Editors

### Cheet sheet

* [devhints.io - Vim cheatsheet](https://devhints.io/vim)
* [Graphical vi-vim Cheat Sheet and Tutorial](http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html)
* [Vim Cheat Sheet](https://vim.rtorr.com/)
* [hackjutsu/vim-cheatsheet](https://github.com/hackjutsu/vim-cheatsheet)

---

> How I Start Using VIM - [a medium blog](https://medium.com/@daviddwlee84/%E6%88%91%E8%88%87vim%E7%B5%90%E5%A9%9A%E4%B8%80%E9%80%B1-%E6%B2%92%E6%9C%89%E5%B9%B4-d6420eda4b8d)
