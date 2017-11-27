# PACKAGE_NAME

SHORT_DESCRIPTION

# Instructions (DELTE THIS LATER)

To build a new python package that is easily distributable, this template
is provided. It contains the structure needed to make python packages
easily installable with pip (the python package manager). 

To create a new python package from this template simply copy **all** the 
files (including .gitignore) from this directory to your new python project
path and change PACKAGE_NAME to a suitable package name. Besides renaming the
folder and the occurences in this README, the name and some other info also
has to be adjusted in `setup.py`.

Afterwards you should push a first commit to your [gitlab](https://gitlab.imr.uni-hannover.de/)
repository. All python code that you write has to be inside the PACKAGE_NAME
directory to be available for import later!

## Installation

To make the contents of this package accessible in other python projects
via `import PACKAGE_NAME`, a `setup.py` file is given. This allows the
user to install the package with pip. For this open a terminal and move
to the top level directory of this repository (the directory containing the
`setup.py` file). Here run

```
pip install [--user] -e .
```

The `-e` stands for editable and causes pip to create a link to the
current working directory in your pythonpath. This means all changes to
the current working directory (either by manual changing of the module,
or by `git pull`) are immeadiatly available for system wide import. For
more information see the [pip install reference](https://pip.pypa.io/en/stable/reference/pip_install/#editable-installs)
and the [Setuptools info page](http://setuptools.readthedocs.io/en/latest/setuptools.html?highlight=development%20mode#development-mode).

