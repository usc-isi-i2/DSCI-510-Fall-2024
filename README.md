# DSCI-510-Fall-2023 - Getting Started


This document explains the things required to get started with programming in python.


## Create a Github account

All students should have a github account, use [this](https://github.com/signup) link to sign up for a new account in case you do not have one.

## Conda: Installation and Virtual Environment setup

[For Windows](https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html)

[For Mac](https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html)

[For Linux](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html)

NOTE: **The following commands are run in a terminal.**

### Creating a virtual environment
Students should create a virtual environment for each assignment, and project in general. This is a good python programming practice. For example, to create a virtual environment for lab assignemnt 1,

```
conda create -n lab-1-env python=3.10 -y
```
Creates a conda virtual environment called `lab-1-env` and the major python version is `3.10`

### Activate the conda environment
```
conda activate lab1-1-env
```

You should see something similar to this ,
```
D22ML-AMANDEEP:~ amandeep$ conda activate lab-1-env
(lab-1-env) D22ML-AMANDEEP:~ amandeep$
```

The (lab-1-env) means that the conda environment: `lab-1-env` is active.

### Check python version
```
python --version
```

Output should be similar to this ,

```
(lab-1-env) D22ML-AMANDEEP:~ amandeep$ python --version
Python 3.10.12
```

### Start Python Shell
Typing the following command in the terminal starts the interactive python shell
```
python
```

The output of the above command should be similar to this ,

```
(lab-1-env) D22ML-AMANDEEP:~ amandeep$ python
Python 3.10.12 (main, Jul  5 2023, 15:02:25) [Clang 14.0.6 ] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Now we are ready to write some code
```
(lab-1-env) D22ML-AMANDEEP:~ amandeep$ python
Python 3.10.12 (main, Jul  5 2023, 15:02:25) [Clang 14.0.6 ] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> x = 1
>>> y = x + 5
>>> x
1
>>> y
6
>>> y += 10
>>> y
16
>>>
```

