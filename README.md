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
### From system .exe
In windows the _program_name_.exe can be found in the virtual environment Scripts folder, usually something like (depending on which program is installed):  
- C:\Users\username\miniforge3\envs\my_env\Scripts
- C:\Users\username\anaconda3\envs\my_env\Scripts
- C:\Users\username\miniconda3\envs\my_env\Scripts

To check where the virtual environment has been installed:

```bash

conda env list 
```
Once you've located _program_name_.exe, right-click it to create a shortcut on your desktop.  

### From terminal  
<img width="416" height="606" alt="image" src="https://github.com/user-attachments/assets/26bd5d57-2f60-46e8-b4b5-9fda7c83f086" />  

A more generic way to create a shortcut for the program is to use the following syntax inside a normal shortcut:

**Target (option 1)**
```bash
%windir%\System32\cmd.exe "/K" C:\Users\username\miniforge3\Scripts\activate.bat C:\Users\username\miniforge3\envs\my_env & program_name
```
**Target (option 2)**
```bash
%windir%\System32\cmd.exe "/K" C:\Users\username\miniforge3\Scripts\activate.bat C:\Users\username\miniforge3\envs\my_env & python D:\Path_to_file\program_name.py
```
**Note the Start in**
```bash
%HOMEPATH
```
**Usage**

This line activates miniforge (modify to anaconda or miniconda path depending on which program is installed)
```bash
C:\Users\username\miniforge3\Scripts\activate.bat
```
This line indicates the path of the virtual environment. Use the 'conda env list' command to display all installed paths.
```bash
C:\Users\username\miniforge3\envs\my_env
```
**Option 1**: This line launch the program.
```bash
& program_name
```
If this command does not work, use the **Option 2**: specify the direct path to the program file as well.
```bash
& python D:\Path_to_file\program_name.py
```
In Rubycond use the 'Ctrl + i' shortcut to locate 'rubycond.py'. An in-app window will open displaying several details, including the file's directory.


  
