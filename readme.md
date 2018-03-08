The code is useful for <a href="http://captain.whu.edu.cn/DOTAweb/">DOTA<a> or
<a href="http://captain.whu.edu.cn/ODAI/">ODAI<a>.
### Installation
1. install swig
```
    sudo apt-get install swig
```
2. create the c++ extension for python
```
    swig -c++ -python polyiou.i
    python setup.py build_ext --inplace
```

### Usage
1. For read and visualize data, you can use DOTA.py
2. For evaluation the result, you can refer to the "dota_evaluation_task1.py" and "dota_evaluation_task2.py"
3. For split the large image, you can refer to the "ImgSplit"
4. For merge the results detected on the patches, you can refer to the ResultMerge.py

An example is shown in the demo.
The subdirectory of "basepath"(which is used in "DOTA.py", "ImgSplit.py") is in the structure of
```
.
├── images
└── labelTxt
```

