# Master Coding

Vim and his happy friends. Also VSCode stuff plus some good development tools collection!

## VIM

Guides

* [Beginner](VIM/BeginnerGuide.md)
* [Intermediate to Master](VIM/AdvancedGuide.md)

Others

* [Key Bind](VIM/KeyBind.md)
* [Dotfile](VIM/dotfile.md)
* [The VimScript](VIM/vimscript.md)
* [Snippet](VIM/snippet.md)
* [NeoVim](VIM/NeoVim.md)
* [VimEverywhere](VIM/VimEverywhere.md)

### Best Friends

* [zsh](VIM/Friends/zsh.md)
* [tmux](VIM/Friends/tmux.md)

### Happy Friends

* [ctags & cscope](VIM/Friends/ctags_cscope.md)

### [Plugin](VIM/Plugin.md)

Plugin Manager

* [vim-plug](https://github.com/junegunn/vim-plug)
* Vundle -> used to use this, but going to switch to ([benifit](https://www.reddit.com/r/vim/comments/4qo7ur/which_plugin_installer_or_vim_package_manager/d4vbaa8)
* NeoBundle
* VimPlug
* Pathogen
* dein

Plugin

* NERDTree - a tree explorer plugin
* YouCompleteMe - a code-completion engine
* surround - quoting/parenthesizing made simple
* fugitive - a git wrapper
* syntastic - syntax checking
* Tagbar - displays tags in a window, ordered by scope
* [ack](https://github.com/mileszs/ack.vim) - a better version of grep in vim
* [easymotion](https://github.com/easymotion/vim-easymotion) - Vim motions on speed!
* Switch input method when switch mode
  * [SmartIM](https://github.com/ybian/smartim/)
    * [vim 中文輸入解決方案](https://zhuanlan.zhihu.com/p/23939198)
  * [vim-xkbswitch](https://github.com/lyokha/vim-xkbswitch)
    * [解決惱人的 vim 中文輸入法切換問題](https://zhuanlan.zhihu.com/p/49411224)
  * [fcitx.vim](https://github.com/vim-scripts/fcitx.vim)
    * [fcitx-vim-osx](https://github.com/dangxuandev/fcitx-vim-osx)
      * [fcitx-remote-for-osx](https://github.com/dangxuandev/fcitx-remote-for-osx)

Collection

* [VimAwesome](https://vimawesome.com/)

### [Theme](VIM/Theme.md) (shared with best friend)

* Powerline font

## Visual Studio Code

Guides

* [Tips](VSCode/Tips.md)

### Extension

* [Youtube - My Favorite VS Code Extensions](https://www.youtube.com/watch?v=rH1RTwaAeGc)
* [Youtube - Learning Vim in a Month with Visual Studio Code](https://www.youtube.com/watch?v=_AOW5ThfI9Y)

#### Must Have

* [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
  * [github](https://github.com/VSCodeVim/Vim)
    * [issue .vimrc support #463](https://github.com/VSCodeVim/Vim/issues/463)
      * [vimrc-to-json.py](https://github.com/Sheepolution/vimrc-to-json)
  * easymotion
  * surround

#### General Purpose

* Live Share
* Git History
* Git Project Manager
* GitLens -- Git supercharged
* Markdown All in One
* Python
* Path Intellisense
* Excel Viewer
* [Bookmarks](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarks) - just like Mark in vim

Remote Development

* [sftp](https://marketplace.visualstudio.com/items?itemName=liximomo.sftp)
* [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)  - using ssh
* [vscode-remote](https://aka.ms/vscode-remote)
  * [microsoft/vscode-dev-containers](https://github.com/microsoft/vscode-dev-containers)

#### Special Purpose

* VS Code Jupyter Notebook Previewer
* [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
  * [github](https://github.com/microsoft/vscode-docker)
* Doxygen Documentation Generator
* ESLint
* Formatting Toggle
* LaTeX Workship
* Markdown PDF
* markdownlint
* Mathlab
* R
* React Native Tools
* VSCode 批踢踢 (VSCode PTT)

### Theme

---

## Git

* [Beginner](Git/BeginnerGuide.md)
* [Advanced](Git/AdvancedGuide.md)

### Git GUI Client

* [Sourcetree](https://www.sourcetreeapp.com/)
* [Github Desktop](https://desktop.github.com/)
* [Fork](https://forkapp.io/)
* [Git Tower](https://www.git-tower.com/)

iOS

* Clone

## Linux

* Productive Tools
  * fzf
* File Manager
  * [Midnight Commander](https://midnight-commander.org/)
* [Terminal / Command Line](Linux/Terminal.md)

## Google Chrome

> [extension store](https://chrome.google.com/webstore/category/extensions)

* [dinosour](chrome://dino/)

Web Debug

* [VisBug](https://chrome.google.com/webstore/detail/visbug/cdockenadnadldjbbgcallicgledbeoc)
* [Wappalyzer](https://www.wappalyzer.com/) - Identify technology on websites

## Taking Notes

### Markdown

Tools

* VSCode + Tab Preview
* MacDown
* Typora

Transfer to pdf

* [pandoc](https://pandoc.org)
  * [manual](https://pandoc.org/MANUAL.html)

Tips

* [Art of README](https://github.com/noffle/art-of-readme)

### LaTeX

* [LaTeX](NoteTaking/LaTeX.md)

(TODO) Seperate notes like tools, Bibtex....

TeX Distribution

* Ubuntu: `sudo apt-get install texlive-full`
* Mac: [MacTeX](http://tug.org/mactex/)
* Windows: [TeX Live](http://tug.org/texlive/) ([instruction](https://liam.page/texlive))

Tools

* VSCode + Tab Preview

Alternative

* Word + [WordTex](https://www.andrew.cmu.edu/user/twildenh/wordtex/)
  * [YouTube - WordTeX - A WYSIPCTWOTCG Typesetting Tool](https://www.youtube.com/watch?v=jlX_pThh7z8)

### Mind Map

* XMind

### Handwriting on iPad

App (Recommend)

* GoodNotes 4

App (Others)

* GoodNotes 5
* Nebo

## Python

* [Understanding the Python Traceback](https://realpython.com/python-traceback/)

### [Jupyter Notebook](Other/JupyterNotebook.md)

* [Jupyter Notebook](https://jupyter.org/)

> * Kaggle Kernel
> * Google Colab

#### Jupyter Extension

* [Jupyter notebook extensions](https://github.com/ipython-contrib/jupyter_contrib_nbextensions) - [Document](http://jupyter-contrib-nbextensions.readthedocs.io/en/latest)
  * Installation: `pip install jupyter_contrib_nbextensions`
  * [Select CodeMirror Keymap](https://github.com/ipython-contrib/jupyter_contrib_nbextensions/tree/master/src/jupyter_contrib_nbextensions/nbextensions/select_keymap) - Enable VIM Mode

### Python Debug

* [PySnooper](https://github.com/cool-RR/PySnooper)

#### Debugger

[Python Debugging Tools Collection](https://wiki.python.org/moin/PythonDebuggingTools)

* [pdb](https://docs.python.org/3/library/pdb.html)
* [**ipdb**](https://github.com/gotcha/ipdb)
  * `import ipdb; ipdb.set_trace() # BREAKPOINT`
  * [Debugging with ipython and ipdb](https://gist.github.com/mono0926/6326015)
    * [slides](https://docs.google.com/presentation/d/1c6BaV6T57z8UjkEd32xQErMtLT0fC-mZOCRaCcP7dcs/edit#slide=id.p)
  * [使用IPDB調試Python代碼](https://xmfbit.github.io/2017/08/21/debugging-with-ipdb/)
* [traceback](https://docs.python.org/3/library/traceback.html)
  * `traceback.print_exc()`

### Python Tricks

Virtual Environment

* `virtualenv`
  * [Python — Virtualenv虛擬環境安裝](https://medium.com/python4u/python-virtualenv%E8%99%9B%E6%93%AC%E7%92%B0%E5%A2%83%E5%AE%89%E8%A3%9D-9d6be2d45db9)
* use conda

Professional CLI Application

* [`argparse`](https://docs.python.org/3.7/library/argparse.html)
* [`docopt`](http://docopt.org/)
  * [docopt/docopt: Pythonic command line arguments parser, that will make you smile](https://github.com/docopt/docopt)
* `fire`
* `click`
* `fabric`, `invoke`

> [Comparing Python Command-Line Parsing Libraries – Argparse, Docopt, and Click – Real Python](https://realpython.com/comparing-python-command-line-parsing-libraries-argparse-docopt-click/)

Logging

* `logging`

Preserve Object

* `pickle`
* `json`, `yaml`

Visualization

> * [Overview of Python Visualization Tools](https://pbpython.com/visualization-tools-1.html)
> * [plotnine：python數據可視化版ggplot2](https://zhuanlan.zhihu.com/p/47814353)

* `matplotlib`
* `pandas' builtin-plotting`
* `seaborn`
* `ggplot`
* `Bokeh`
* `plotly`
* [`visdom`](https://github.com/facebookresearch/visdom)

> LaTeX Plot
>
> * [nschloe/tikzplotlib: Convert matplotlib figures to TikZ/PGFplots for smooth integration into LaTeX.](https://github.com/nschloe/tikzplotlib)

Hide process name from `top` or `ps -aux | grep python`

* `setproctitle`

  ```py
  from setproctitle import setproctitle, getproctitle
  procname = 'Hello World!'
  setproctitle(procname)
  print(getproctitle())
  # Your Code
  ```

Notification

* [SeTeM/pync: Python wrapper for Mac OS 10.8 Notification Center](https://github.com/SeTeM/pync)
* [jaredks/rumps: Ridiculously Uncomplicated macOS Python Statusbar apps](https://github.com/jaredks/rumps)

Schedule

* [Python | Schedule Library - GeeksforGeeks](https://www.geeksforgeeks.org/python-schedule-library/)

Configuration

* [google/gin-config: Gin provides a lightweight configuration framework for Python](https://github.com/google/gin-config)

> * [chiphuyen/python-is-cool: Cool Python features for machine learning that I used to be too afraid to use](https://github.com/chiphuyen/python-is-cool)

---

## Learning Resources

* [CodeCademy](https://www.codecademy.com/)
* [Upcase](https://thoughtbot.com/upcase)

Python

* [Kaggle Learn Python](https://www.kaggle.com/learn/python)
* [jackfrued/Python-100-Days](https://github.com/jackfrued/Python-100-Days) - Chinese Python resource

Game

* [lettier/3d-game-shaders-for-beginners](https://github.com/lettier/3d-game-shaders-for-beginners)

## Other Notes

* [ivmm/Student-resources](https://github.com/ivmm/Student-resources)
* [Break GFW](Other/BreakGFW.md) - VPN, proxy...

### To Be Productive

* [Tricks](Productivity/Tricks.md)

Tools

* Time Management
  * Pomodoro Technique
    * Pomotodo
* Team/Project Management
  * Kanban
    * Trello
    * GitHub build-in Projects
    * Jira
  * Gantt Chart

### Computing Resources

* [Intel® AI DevCloud](https://software.intel.com/en-us/ai/devcloud)

### Coding Style

Python

* [You (Probably) Don’t Need For-Loops - Python Pandemonium - Medium](https://medium.com/python-pandemonium/never-write-for-loops-again-91a5a4c84baf)
* Google
  * [styleguide | Style guides for Google-originated open-source projects](https://google.github.io/styleguide/pyguide.html)
  * [.pylintrc](https://github.com/google/seq2seq/blob/master/pylintrc)
  * [google/yapf: A formatter for Python files](https://github.com/google/yapf)

#### Formatter, Prettifier

JavaScript

* [google/code-prettify](https://github.com/google/code-prettify) - JavaScript code prettifier
* [Prettier](https://prettier.io/)
  * [prettier/prettier](https://github.com/prettier/prettier)

### Summary

* [Programming Technology Tree](XMind/ProgrammingTechnologyTree.xmind) - My XMind Mind Map noting almost every trivial things about programming since early 2018.

#### Web Development

```txt
<             Front-end Engineer            >
          <               Back-end Engineer             >
                             <          Algorithm Engineer          >
| UI / UX | Front-end Logic | Back-end Logic | Database | Algorithm |
```

---

## GUI Tools Collection

### Better Terminal

* [**iTerm2**](https://www.iterm2.com/) - Mac OS X
* [**Windows Terminal**](https://github.com/microsoft/Terminal) - It's open source and just released on Github in early May, 2019. (will delivered in Windows Store)
* [Hyper](https://hyper.is/) - Cross Platform
* [Fluent Terminal](https://github.com/felixse/FluentTerminal) - Terminal for PowerShell, CMD, WSL or custom shells

### API

* [Postman](https://www.getpostman.com/)
* [Insomnia](https://www.insomnia.rest/)

### Other

* Dash (including MacOS, iOS, VSCode client)
* [SwitchHost](https://oldj.github.io/SwitchHosts/) - hosts management & switching
* [KeeWeb](https://keeweb.info/) - cross-platform password manager

#### Code Presentation

* [pastebin](https://pastebin.com/)
  * pastebinit

## CLI Tools Collection

### Useless Tools

* cowsay
* [FIGlet](http://www.figlet.org/) - display large characters made up of ordinary screen characters
  * [github](https://github.com/cmatsuoka/figlet)
  * [a good example](https://gist.github.com/LunaCodeGirl/6707775)
* toilet - display large colourful characters
* fortune - print a random, hopefully interesting, adage
* lolcat - rainbow coloring effect for text console display

```sh
$ fortune | cowsay | lolcat -a
$ echo "KTHXBAI" | toilet | lolcat
$ date | figlet -k
```

### Reverse Proxy

> 內網穿透

* [ngork](https://ngrok.com/)- public URLs for localhost
* [fatedier/frp](https://github.com/fatedier/frp) - A fast reverse proxy to help you expose a local server behind a NAT or firewall to the internet
* [NGINX](https://www.nginx.com/) - High Performance Load Balancer, Web Server, & Reverse Proxy

### Slides

* [patat](https://github.com/jaspervdj/patat)
* [tpp](https://github.com/cbbrowne/tpp)

### Browser

> * [Browsing the internet from the command line](https://askubuntu.com/questions/29540/browsing-the-internet-from-the-command-line)

* ELinks
* Lynx
  * `sudo apt-get install lynx-cur`
* w3m
  * `sudo apt-get install w3m w3m-img`

### Monitor

* top / htop

## iOS Tools Collection

* Termius
* Pythonista with StaSh
* Fing
* POP

---

## Other Tools Collection

* Text Editor
  * CLI
    * Emacs
    * Nano
  * Cross-platform
    * Sublime
    * Atom
      * [atom-beautify](https://atom.io/packages/atom-beautify)
  * Windows
    * Notepad++
  * OS X
    * [TextMate](https://macromates.com/)
  * Ubuntu
    * gedit
* IDE
  * C/C++
    * Dev C++
    * Code::Blocks
    * [Cevelop](https://www.cevelop.com/)
  * Python
    * PyCharm
  * Embedding
    * Keil C
  * Verilog
    * Xilinx Vivado - Support Windows and Linux
  * Web
    * [Coda](https://panic.com/coda/)
  * General Purpose
    * Visual Studio
    * Eclipse
    * [NetBeans](https://netbeans.org/)
* Emulator
  * Linux
    * Cygwin
  * Android
    * [Bluestacks 4](https://www.bluestacks.com/tw/index.html)
      * [China version](https://www.bluestacks.cn/) (Windows only)
    * [NoxPlayer](https://tw.bignox.com/)
    * [Droid 4x](https://droid4x.cc/) (Windows only)
      * [official](https://droid4xofficial.com/)
  * Windows
    * wine - [wine notes](Other/wine.md)
  * DOS
    * DOSBox
      * `brew cask install dosbox`
* Browser
  * Google Chrome
    * User Script - [Install User Script](https://greasyfork.org/en/help/installing-user-scripts)
      * [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
* Remote Control
  * CLI
    * PuTTY
    * [MobaXterm](https://mobaxterm.mobatek.net/) - Enhanced terminal for Windows with X11 server, tabbed SSH client, network tools
    * [ttyd](https://github.com/tsl0922/ttyd) - Share your terminal over the web
  * GUI
    * VNC
* Typing Check
  * [Grammarly](https://www.grammarly.com/)
  * [LanguageTool](https://languagetool.org/)
* Downloader
  * [`aria2c`](https://aria2.github.io/)
    * [github](https://github.com/aria2/aria2)
    * [aria2 設定教學 – 強大又輕巧的下載工具，支援 BT、斷點續傳](https://ibe.tw/aria2/)
  * [NeteaseCloudMusicFlac](https://github.com/YongHaoWu/NeteaseCloudMusicFlac) - Download the FLAC music from NeteaseCloudMusic playlist
* Tester
  * [speedtest-cli](https://github.com/sivel/speedtest-cli) - Command line interface for testing internet bandwidth using speedtest.net
* Design
  * 3D Model (for 3D print)
    * Fusion 360
    * Blender
  * PCB
    * [EasyEDA](https://easyeda.com/)
  * Diagram
    * [draw.io](https://www.draw.io/)
    * [ProcessOn](https://www.processon.com/) - Diagrams, Flowchart, Mindmap
* Make video => GIF
  1. [Gifox](https://gifox.io/) or (⌘⇧5 on Mac)
  2. [ImageOptim](https://imageoptim.com) - reduce the image size (replace the old one)
* Video Editor
  * [Davinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve/)
  * [Adobe Premiere Elements](https://www.adobe.com/tw/products/premiere-elements.html)
  * [Quik](https://shop.gopro.com/International/softwareandapp/quik-%7C-desktop/Quik-Desktop.html)
* Downloader
  * YouTube
    * [FindYoutube.net](https://www.findyoutube.net/)
      * [manual](https://help.findyoutube.net/help)
      * [browser script](https://greasyfork.org/en/scripts/8426-download-youtube-videos-and-subtitles)
* File Transfer
  * HTML to PDF
    * [Sejda - Convert HTML to PDF Online](https://www.sejda.com/html-to-pdf)
    * [HTML to PDF – Convert HTML files to PDF](https://html2pdf.com/)
* Slides
  * [GitPitch - The Markdown Presentation Service on Git.](https://gitpitch.com/)
  * HTML
    * [reveal.js – The HTML Presentation Framework](https://revealjs.com/#/)
  * Markdown
    * [hiroppy/fusuma: ✍️Fusuma makes slides with Markdown easily.](https://github.com/hiroppy/fusuma)
* Coooooool Stuff
  * [Camelot: PDF Table Extraction for Humans](https://github.com/atlanhq/camelot)
    * [Command-Line Interface](https://camelot-py.readthedocs.io/en/master/user/cli.html)
  * [Anime4K: A High-Quality Real Time Upscaler for Anime Video](https://github.com/bloc97/Anime4K)
  * [Gapplin - SVG Viewer for macOS](http://gapplin.wolfrosch.com/)
  * [PyGithub/PyGithub: Typed interactions with the GitHub API v3](https://github.com/PyGithub/PyGithub)
  * [Zotero | Your personal research assistant](https://www.zotero.org/)

### Script

* Baidu Drive
  * [houtianze/bypy](https://github.com/houtianze/bypy) - Python client for Baidu Yun
  * [peterq/pan-light](https://github.com/peterq/pan-light)
