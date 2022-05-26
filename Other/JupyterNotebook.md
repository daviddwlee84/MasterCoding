# Jupyter Notebook

## Installation and Basic Usage

### As Local Editor

Installation

```sh
pip3 install jupyterlab
```

> Classic Notebook
>
> ```sh
> python3 -m pip install --upgrade pip
> python3 -m pip install jupyter
> ```

Usage

```sh
# Local web server
jupyter notebook
ipython notebook

# Jupyter Lab web server
jupyter-lab

# CLI
ipython
```

### As Server

#### Use ssh tunnel

1. Open jupyter notebook on remote server
   1. connect to remote server `ssh $REMOTE_USER@$REMOTE_IP`
   2. run jupyter `jupyter notebook`
2. `ssh -NfL $LOCAL_PORT:localhost:$REMOTE_PORT $REMOTE_USER@$REMOTE_IP > /dev/null 2>&1`

## Extensions

* [Unofficial Jupyter Notebook Extensions - jupyter_contrib_nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/index.html)
* [ipython-contrib/jupyter_contrib_nbextensions: A collection of various notebook extensions for Jupyter](https://github.com/ipython-contrib/jupyter_contrib_nbextensions)

```sh
# Install the python package
pip3 install jupyter_contrib_nbextensions

# Install javascript and css files
jupyter contrib nbextension install --user
```

* [Jupyter-contrib/jupyter_nbextensions_configurator](https://github.com/Jupyter-contrib/jupyter_nbextensions_configurator): A jupyter notebook serverextension providing config interfaces for [nbextensions](https://github.com/ipython-contrib/jupyter_contrib_nbextensions). => enable options (front-end interface) in Jupyter Notebook ([http://localhost:8889/tree?#nbextensions_configurator](http://localhost:8889/tree?#nbextensions_configurator))

```sh
# Installing the pip package
pip install jupyter_nbextensions_configurator

# Configuring the notebook server to load the server extension
jupyter nbextensions_configurator enable --user
```

> Edit > nbextensions config

Must enable

* Select CodeMirror Keymap
    > Edit > Keymaps > Vim
* Hinterland - Autocompletion
* highlighter - Highlight the markdown notes
* ExecuteTime
* Code prettify
* Notify

Optional

* Codefolding

## Tips

### Execute Notebook in Terminal

> [python - How to run an .ipynb Jupyter Notebook from terminal? - Stack Overflow](https://stackoverflow.com/questions/35545402/how-to-run-an-ipynb-jupyter-notebook-from-terminal)

```sh
alias nbx="jupyter nbconvert --execute --to notebook"
nbx [--inplace] <notebook>
```

### Magic Commends

`%Ismagic`

## Kernel for other languages

### Kernel for Go

> make sure you've set `$GOPATH` and add `$GOPATH/bin` in your `$PATH`

* [gopherdata/gophernotes: The Go kernel for Jupyter notebooks and nteract.](https://github.com/gopherdata/gophernotes)

### Kernel for C++

* [QuantStack/xeus-cling](https://github.com/QuantStack/xeus-cling/)
  * [document](https://xeus-cling.readthedocs.io/en/latest/)

## Resources

* [How to get autocomplete in jupyter notebook without using tab?](https://stackoverflow.com/questions/45390326/how-to-get-autocomplete-in-jupyter-notebook-without-using-tab/)
* [Can I run Jupyter notebook cells in commandline?](https://stackoverflow.com/questions/35471894/can-i-run-jupyter-notebook-cells-in-commandline)
  * runipy
    * `pip3 install runipy`
    * `runipy MyNotebook.ipynb`
    * `runipy MyNotebook.ipynb OutputNotebook.ipynb`
    * `runipy MyNotebook.ipynb --html report.html`
  * jupyter nbconvert
    * `jupyter nbconvert --to notebook --inplace --execute mynotebook.ipynb`
* [Change the Theme in Jupyter Notebook?](https://stackoverflow.com/questions/46510192/change-the-theme-in-jupyter-notebook)
  * `pip3 install jupyterthemes`
  * `jt -t <theme-name>`
    * onedork
    * grade3
    * oceans16
    * chesterish
    * monokai
    * solarizedl
    * solarizedd

### Jupyter Family

* [jupyter/notebook: Jupyter Interactive Notebook](https://github.com/jupyter/notebook)
* [jupyterlab/jupyterlab: JupyterLab computational environment.](https://github.com/jupyterlab/jupyterlab)
* [jupyterhub/jupyterhub: Multi-user server for Jupyter notebooks](https://github.com/jupyterhub/jupyterhub)

Tools

* [datitran/jupyter2slides: Cloud Native Presentation Slides with Jupyter Notebook + Reveal.js](https://github.com/datitran/jupyter2slides)
* [dunovank/jupyter-themes: Custom Jupyter Notebook Themes](https://github.com/dunovank/jupyter-themes)

### Similar Online Editor

> * [Six easy ways to run your Jupyter Notebook in the cloud](https://www.dataschool.io/cloud-services-for-jupyter-notebook/)

* Kaggle Kernel
* [Google Colab](https://colab.research.google.com/)
  * [googlecolab/colabtools: Python libraries for Google Colaboratory](https://github.com/googlecolab/colabtools)
* BinderBinder
* [Binder](https://mybinder.org/)
* Microsoft Azure Notebooks
* [CoCalc - Online Jupyter Notebooks](https://cocalc.com/doc/jupyter-notebook.html) - Support Co-work (need to pay)
* Datalore

### Alternative

* [**nteract: write your next code-driven story.**](https://nteract.io/) => open notebook directly through double click
  * [github](https://github.com/nteract/nteract)
* [aaren/notedown: Markdown <=> IPython Notebook](https://github.com/aaren/notedown) - Use markdown to write jupyter notebook
  * [szymonmaszke/vimpyter: Edit your Jupyter notebooks in Vim/Neovim](https://github.com/szymonmaszke/vimpyter)
