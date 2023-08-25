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
conda activate lab-1-env
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

Press `Enter` to execute a line in the python shell.

## IDE Recommendation

Students can download a one year free license for [PyCharm](https://www.jetbrains.com/community/education/#students) with USC email id. I use `PyCharm` myself in my projects.
You do not have to use `PyCharm`, any text editor would work.

## Installing Jupyter Lab

Jupyter lab provides a web based interactive development environment. Install jupyter lab by running this command, in the terminal ,

```
pip install jupyterlab
```

You will have to register your conda environment with Jupyter before it can be used in the jupyter notebooks. If the conda environment
is called `lab-1-env`,  run the following command to register this conda environment with Jupter ,

```
python -m ipykernel install --name lab-1-env --display-name lab-1-env
```

Finally, run jupyter lab by typing the following command ,

```
jupyter lab
```

You should see output similar to this ,

```
https://jupyter-notebook.readthedocs.io/en/latest/migrate_to_notebook7.html

Please note that updating to Notebook 7 might break some of your extensions.

[I 2023-08-14 16:53:33.035 ServerApp] nbclassic | extension was successfully loaded.
[I 2023-08-14 16:53:33.035 ServerApp] Serving notebooks from local directory: /Users/amandeep/Downloads/DSCI 510 - Fall 2022/lectures/week 1
[I 2023-08-14 16:53:33.036 ServerApp] Jupyter Server 2.1.0 is running at:
[I 2023-08-14 16:53:33.036 ServerApp] http://localhost:8888/lab?token=ddb241eb40394243ea17d0bb252d89d3d973bc198c2780b5
[I 2023-08-14 16:53:33.036 ServerApp]  or http://127.0.0.1:8888/lab?token=ddb241eb40394243ea17d0bb252d89d3d973bc198c2780b5
[I 2023-08-14 16:53:33.036 ServerApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 2023-08-14 16:53:33.038 ServerApp]

    To access the server, open this file in a browser:
        file:///Users/amandeep/Library/Jupyter/runtime/jpserver-48598-open.html
    Or copy and paste one of these URLs:
        http://localhost:8888/lab?token=ddb241eb40394243ea17d0bb252d89d3d973bc198c2780b5
     or http://127.0.0.1:8888/lab?token=ddb241eb40394243ea17d0bb252d89d3d973bc198c2780b5
[I 2023-08-14 16:53:36.114 LabApp] Build is up to date
```

