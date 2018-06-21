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
3. Save it with a meaningful name like: **Python3.sublime-build**
4. Go to **Sublime Text** : *Tools -> Build system ->* and check Python3
5. Paste code below and save as python file:
```PYTHON
import sys
print(sys.version)
```
6. Test if executable press : **Ctrl + b**

***
#### How to Install Module for Specific Python Version
```CMD
python2 -m pip install ModuleName1 ModuleName2 ...
```

```CMD
python3 -m pip install ModuleName1 ModuleName2 ...
```
