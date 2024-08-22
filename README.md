# PyOllyTutorial
Basic Python for Data

***
## Other Hand Out
#### Chat Sheet List for Data Scientists
* [Python for Beginners](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/PythonForDataScience.pdf)
* [Pandas 1](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/PandasPythonForDataScience.pdf), [Pandas 2](https://www.dataquest.io/blog/images/cheat-sheets/pandas-cheat-sheet.pdf), [Pandas Advance](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Pandas_Cheat_Sheet_2.pdf)
* [Numpy 1](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Numpy_Python_Cheat_Sheet.pdf), [Numpy 2](https://www.dataquest.io/blog/images/cheat-sheets/numpy-cheat-sheet.pdf)
* [ScipPy](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_SciPy_Cheat_Sheet_Linear_Algebra.pdf)
* [Matplotlib](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Matplotlib_Cheat_Sheet.pdf)
* [Bokeh](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Bokeh_Cheat_Sheet.pdf)
* [Scikit-Learn](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Scikit_Learn_Cheat_Sheet_Python.pdf)
* [PySpark](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/PySpark_Cheat_Sheet_Python.pdf)
* [Keras](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Keras_Cheat_Sheet_Python.pdf)



***
#### Miniconda Jupyter Notebook Installation
1. Install [Miniconda](https://conda.io/en/latest/miniconda.html)
2. Install Jupyter in Anaconda Prompt CMD :
```CMD
pip install jupyter
```
3. Create Python/R Kernel with essentials package
```CMD
conda create -n myenv python=3.12
```
```CMD
conda create -n myenv r r-essentials 
```
4. Activate/Deactivate Kernel
```CMD
conda activate myenv
```
```CMD
conda deactivate
```
5. Install Module/packages within activated kernel
```CMD
conda install openpyxl sqlalchemy pyodbc pyhive opencv numpy scipy sympy pandas matplotlib requests lxml patsy scikit-learn xlrd requests BeautifulSoup4 bokeh
```
```CMD
conda install r-irkernel
```
6. Install Jupyter Notebook within activated kernel
```CMD
conda install jupyter
```
7. Remove Env
```CMD
conda remove --name myenv --all
```
8. Add Env into Kernal in Jupyter Notbook
```CMD
activate myenv
pip install ipykernel
python -m ipykernel install --user --name myenv --display-name "Python (whatever you want to call it)"
```
10. Remove Kernal in Jupyter Notebook
```CMD
jupyter kernelspec list
jupyter kernelspec remove <kernel_name>
```
12. More Info [Conda info](https://www.geeksforgeeks.org/how-to-install-jupyter-notebook-in-windows/) / [Conda Chat Sheet](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)

***
#### How to Link Sublime Text Build System to Python
1. Go to **Sublime Text** : *Tools -> Build System -> New Build System* 
2. Paste code as below:
```JSON
{
    "cmd": ["python3", "-i", "-u", "$file"],
    "file_regex": "^[ ]File \"(...?)\", line ([0-9]*)",
    "selector": "source.python"
}
```
(if want to use conda env use below code instead)
```CMD
{
    "cmd": ["C:\\Users\\sschen\\.conda\\envs\\myenv\\python.exe", "-u", "$file"],
    "file_regex": "^[ ]File \"(...?)\", line ([0-9]*)",
    "selector": "source.python"
}
```
3. Save it with a meaningful name like: **Python3.sublime-build**
4. Go to **Sublime Text** : *Tools -> Build system ->* and check Python3
5. Paste code below and save as python file:
```PYTHON
import sys
print(sys.version)
```
6. Test if executable press : **Ctrl + b**



***
#### How to Set Personalized "Pause Key" in Sublime
1. Go to **Sublime Text** : *Preference -> Key Bindings-User* 
2. Paste code as below:
```JSON
{"keys": ["ctrl+shift+c"], "command": "exec", "args": {"kill": true} } 
```
3. Save it
4. Test if executable press : **Ctrl + Shift + c**



***
#### Sublime Hot Key
1. Select whole line : **Ctrl + l**
2. Push forward/back : **Ctrl+ [** / **Ctrl + ]**
3. Edit all keyword : select one of your word  then **Alt + F3**
4. Edit part of keyword : select one of your word then **Ctrl + d **
5. Delete one line : **Ctrl + x**
6. Add one line above/below : **Ctrl + Shift + Enter** / **Ctrl + Enter**



***
#### How to Install Module for Specific Python Version
```CMD
python2 -m pip install ModuleName1 ModuleName2 ...
```

```CMD
python3 -m pip install ModuleName1 ModuleName2 ...
```
OR
```CMD
python3 -m pip --proxy http://XX.X.XX.XX:8080 install ModuleName1 ModuleName2
```

***
#### How to Add Virtual Env for Python
The Env path should be at the path you did cmd in defult
```CMD
python -m venv EnvName
```
```CMD
EnvName\Scripts\activate
```
```CMD
deactivate
```
