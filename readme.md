The code is useful for <a href="http://captain.whu.edu.cn/DOTAweb/">DOTA<a> or
<a href="http://captain.whu.edu.cn/ODAI/">ODAI<a>.

### Description
<p>
Dota is a large-scale dataset for object detection in aerial images. 
It can be used to develop and evaluate object detectors in aerial images. 
We will continue to update DOTA, to grow in size and scope and to reflect evolving real-world conditions.
For the <strong style="color:blue"> DOTA-v1.0</strong>, as described in the 
<a href="https://arxiv.org/abs/1711.10398">paper</a>, it contains <strong style="color:blue">2806</strong>  aerial images from different sensors and platforms. 
Each image is of the size in the range from about <strong style="color:blue"> 800 &times 800 to 4000 &times 4000 </strong>  pixels
and contains objects exhibiting a wide variety of scales, orientations, and shapes. These DOTA images are then annotated
by experts in aerial image interpretation using 15 common object categories. The fully annotated DOTA images 
contains <strong style="color:blue">188, 282</strong> instances, each of which is labeled by an arbitrary (8 d.o.f.) quadrilateral.
</p>

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

