## Install virtual environment

1) Download and install [Miniforge](https://github.com/conda-forge/miniforge)  
   Anaconda and Miniconda work the same way, but Miniconda uses free and openly-licensed packages from the conda-forge project by default. [More info.](https://www.sens.buffalo.edu/software/conda)

2) From miniforge/anaconda prompt (windows) or terminal (Ubuntu & MAC) create a virtual environment with name _my_env_:

```bash
conda create -n  my_env pip
```

3) Activate the virtual environment _my_env_ with
```bash
conda activate my_env
```

4) Install _program_name_ with:

```bash
pip install program_name
```

5) Launch _program_name_ in terminal:

```bash
program_name
```
6) Deactivate the virtual environment _my_env_ with

```bash
deactivate
```
7) Delete the virtual environment _my_env_ with

```bash
conda remove -n my_env --all
```
## Shortcut

In windows the _program_name_.exe can be found in the virtual environment Scripts folder, usually something like:  
- C:\Users\username\anaconda3\envs\my_env\Scripts
- C:\Users\username\miniconda\envs\my_env\Scripts

To check where the virtual environment has been installed:

```bash

conda env list 
```
