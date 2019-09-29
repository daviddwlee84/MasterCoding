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
# open local web server
jupyter notebook
ipython notebook

# CLI
ipython
```

### As Server

## Extensions

### [Unofficial Jupyter Notebook Extensions - jupyter_contrib_nbextensions](https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/index.html)

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

## Kernel for C++

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

### Similar Online Editor

* Kaggle Kernel
* [Google Colab](https://colab.research.google.com/)
