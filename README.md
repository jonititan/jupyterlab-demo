# JupyterLab Demonstration
This Repo is intended to make it easy to create interactive worked examples for [Project Rho](http://www.projectrho.com/public_html/rocket/index.php)
[![Binder](https://beta.mybinder.org/badge.svg)](https://mybinder.org/v2/gh/jonititan/projectrho-lab/master?urlpath=lab/tree/demo/Lorenz.ipynb)

This repo borrows heavily from the reference demo for jupyterlab and could not exist without it.


## Installation

The demo requires [conda](https://conda.io/miniconda.html) and the package
 requirements are described in `environment.yml`

To install the environment and demofiles, we use [pyinvoke](http://pyinvoke.org). To install pyinvoke with conda call:

```bash
conda install -c conda-forge invoke pyyaml
```

### Create the environment

To create the conda environment with all the dependencies and jupyterlab extensions for the demo, run:

```bash
invoke environment  # optionally --env-name=my-env-name
```

The default environment name is `projectrho-lab`.

To create the environment and remove previous installation, call:

```bash
invoke environment --clean
```

### Activate/deactivate the environment

To activate the conda environment, run:

```bash
source activate projectrho-lab
```

To deactivate the conda environment, run:

```bash
source deactivate
```

### R Language support

To add R language support, run:

```bash
invoke r
```

### Julia Language support

To add Julia language support follow the instructions [here](https://github.com/JuliaLang/IJulia.jl#installation).


### Uninstalling

To uninstall the demofiles and enviornment, call:

```
invoke clean
```

# Demo guide

The basic outline of the JupyterLab demo is described in the file `projectrholab.md`.


