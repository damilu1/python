## 学习numpy，记录笔记

```python
import numpy as np

print(type(x))  #打印数组x的数据类型（list,dict,numpy.ndarray）
print(x.shape)  #打印数组x的形状
print(x.dtype)  #打印数组x中元素的数据类型（int,float）；其中list,dict等可以包含不同的数据类型，因此不可调用x.dtype方法；numpy.array中要求所有元素属于同一数据类型，因此可调用x.dtype方法
print(x.size)   #打印数组x的尺寸（数组元素的总数）
print(x.ndim)   #打印数组x的维数


```
#### numpy.ndarray与numpy.matrix的区别
ndarray 可以是任意维数 mat只能是2维的
