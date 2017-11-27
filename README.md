# PACKAGE_NAME

SHORT_DESCRIPTION

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

