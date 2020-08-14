## 记录Matplotlib笔记
### Matplotlib函数总结


**kwargs与args**
```python
from matplotlib import pyplot as plt #导入matplotlib文件中的pyplot.py  (import matplotlib.pyplot as plt)

plt.figure(num="int"or"str",figsize=(float,float),dpi=float)    #设置图像窗口的参数（图像名字，图像大小，分辨率）

plt.plot(x,y,format_string, **kwargs)      #绘制图像（x,y坐标轴，控制曲线的格式字符串，更多条曲线(x,y,format_string)）




plt.show() #展示图像

```



# 记录Matplotlib笔记
## Matplotlib函数总结：
```python
from matplotlib import pyplot as plt #导入matplotlib文件中的pyplot.py  (import matplotlib.pyplot as plt)

plt.figure(num="int"or"str",figsize=(float,float),dpi=float)    #设置图像窗口的参数（图像名字，图像大小，分辨率）

plt.plot(x,y,format_string, **kwargs)      #绘制图像（x,y坐标轴，控制曲线的格式字符串，更多条曲线(x,y,format_string)）

plt.show() #展示图像

```

>## Matplotlib相关问题：
1.kwargs与args之间的关系？



