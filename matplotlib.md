# 记录Matplotlib笔记
>## 一、Matplotlib函数总结：
```python
from matplotlib import pyplot as plt #导入matplotlib文件中的pyplot.py画图模块  (import matplotlib.pyplot as plt)
from matplotlib import font_manager #导入matplotlib文件中的font_manager.py字体管理模块



plt.figure(num="int"or"str",figsize=(float,float),dpi=float)    #设置图像窗口的参数（图像名字，图像大小，分辨率）
plt.plot(x,y,format_string, **kwargs)      #绘制图像（x,y坐标轴，控制曲线的格式字符串--上网查，更多条曲线(x,y,format_string)）

my_font = font_manager.FontProperties(fname="C:\Windows\Fonts\SIMFANG.TTF") #采用系统文件中的中文格式
plt.xticks(range, labels, rotation, FontProperties=my_font)   #设置x轴刻度（刻度的范围，刻度的标签，刻度的旋转度数，设置中文字体）
plt.savefig("fname")   #在plt.show()之前调用plt.savefig(“路径文件名”)  相比jpg，svg放大后不会失真

plt.show() #展示图像

```

>## 二、Matplotlib相关问题：
* \*args与\*\*kwargs之间的关系和区别？



