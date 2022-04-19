# Diabetes Factors Analysis

## Setting up running environment (with conda)

### Install Conda

#### Windows / Mac

[Anaconda installer for Windows](https://www.anaconda.com/products/individual "Anaconda installer for Windows")

#### Linux

```bash
wget https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh
bash Anaconda-latest-Linux-x86_64.sh
```

### Set up for conda-forge

```bash
conda config --add channels conda-forge
```

### Set up conda environment

```bash
conda create -n r_env # with environment name r_env as example
conda activate r_env
```

### Install package

```bash
conda install -c conda-forge r-recommended r-irkernel r-languageserver
conda install -c conda-forge r-recommended radian # optional
conda install -c conda-forge Jupyter
```

### Install R package

```bash
conda install -c r r-rpart
conda install -c conda-forge r-dplyr r-ggplot2 r-haven 
conda install -c conda-forge r-rpart.plot r-hrbrthemes r-reshape2
```

## Assign Radian as the default R in Linux (optional)

```bash
alias r="radian"
```

## Setting up running environment (without conda)

### Install R

[Download and Install R](https://cloud.r-project.org/ "Download and Install R")

### Install Python

[Download and Install Python](https://www.python.org/downloads/ "Download and Install Python")

### Install Radian (optional)

```bash
pip3 install -U radian
```

## Assign Radian as the default R in Linux (optional)

```bash
alias r="radian"
```

### Install R package

```bash
radian # r if you did not install radian
```

```R
install.packages("dplyr")
install.packages("ggplot2")
install.packages("haven")
install.packages("hrbrthemes")
install.packages("reshape2")
install.packages("rpart")
install.packages("rpart.plot")
quit()
```

## Setup the R kernel

### Setup the R kernel for Jupyter in Linux

```bash
radian # r if you did not install radian
```

```R
IRkernel::installspec()
quit()
```

### Download this repository

```bash
git https://github.com/AlexLeungZ/SDSC2102-project.git
```

### Setup in VScode (Optional)

[VS code](markdown/vscode.md)

### Choosing R as Jupyter kernel

### Try running a test code

1. Run the code ```r_test.ipynb```

## Credits

[Conda Docs](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html "Conda Docs")

[Conda-forge](https://conda-forge.org/docs/user/introduction.html "Conda-forge")

[Radian](https://github.com/randy3k/radian "Radian")
