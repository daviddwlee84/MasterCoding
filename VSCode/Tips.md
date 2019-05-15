# Visual Studio Code Tips

## Comand Bar

* `Command + p` to trigger. Type `?` in it to get help

### Quick open file

* `Command + p` => `[filename in workspace]`

### Trigger command

* `Command + Shift + p` => In command bar `>[command]` (also work in Sublime)

### Search between Function/Symbol/Tags

* `Command + t` => `#[symbol]`

### Others

> Start with `Command + p`

* Goto line `:[line]` (equivalent to `[line]G` in VIM)
* Select view `view [window name]`
  * `view explorer` (is equivalent to `Command + Shift + e`)
  * `view search` (is equivalent to `Command + Shift + f`)
  * `view source control` (is equivalent to `Ctrl + Shift + g`)
  * `view [other installed extensions]`
  * (`view extension` is equivalent to `ext` and `Command + Shift + x`)

## Selection

### Multiple same pattern selection

* Select a pattern (or will auto select the word under cursor) + `Command + d` × N (also work in Sublime)
  * If use VIM plugin, you can type `d` or `c` after selection to trigger *delete* or *change*.

### Block selection

Just like `Ctrl + v` in VIM.

You can press `Shift + Alt` and then use mouse to select a block area.

## Terminal Related

### Open Terminal

* Open terminal directly (if none will create one): Ctrl + `
* Open bottom window: `Command + j`
* `Command + p` then type `term [listed terminal name / create]`

## My other tricks

### Combo

#### Open a new window with Former workspace

1. `Command + Shift + n` to open new empty window
2. `Ctrl + r` to trigger search bar. Then type the workspace folder name.

#### List installed extension management

1. `Command + p` then type `ext` and press `Enter` to open extension marketplace
2. Type `@installed` to show all the extension that installed with this VSCode

### Other VIM Related tricks

#### Switch window

1. `<Ctrl + w> + h` to go to the Explorer window (or any other window)
2. Navigate the options using `j` and `k`
3. Select item using `l`

## General Keyboard Shortcut (working the same way as other program)

### Navigate Tabs

* `Ctrl + Tab` go to next tab. / `Ctrl + Shift + Tab` to to previous tab. (this will conflict with system shortcut in MacOS)
* `Ctrl + [number]` go to the nth tab

### Close window/tab

* `Command + w` close current tab
