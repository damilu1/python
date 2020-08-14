# 记录Matplotlib笔记
>## 一、Matplotlib函数总结：
```python
from matplotlib import pyplot as plt #导入matplotlib文件中的pyplot.py画图模块  (import matplotlib.pyplot as plt)
from matplotlib import font_manager #导入matplotlib文件中的font_manager.py字体管理模块


#####################创建绘图窗口并绘制图像##########################
#生成绘图窗口（图像名，图像大小，分辨率）
plt.figure(num="int"or"str",figsize=(float,float), dpi=float)

#绘制图像(横纵坐标，曲线格式，数据点格式，透明度)
plt.plot(x, y, linestyle, linewidth, marker, markersize, markerfacecolor, alpha)

############################对绘图窗口进行操作##########################
my_font = font_manager.FontProperties(fname="C:\Windows\Fonts\SIMFANG.TTF") #采用系统文件中的中文格式
#设置x轴刻度（刻度的范围，刻度的标签，刻度的旋转度数，设置中文字体）
plt.xticks(range, _xticks_labels, rotation, FontProperties=my_font)

#添加水印（水印左下角坐标，水印内容，字体格式，透明度）
plt.text(x, y, string, fontsize, color, alpha)

plt.savefig("fname")   #保存图像  在plt.show()之前调用plt.savefig(“路径文件名”)  相比jpg，svg放大后不会失真
plt.show() #展示图像

```
[Matplotlib中的颜色、线条、标记样式汇总(感谢知乎大佬Mr.喵)](https://zhuanlan.zhihu.com/p/40992563)

>## 二、Matplotlib相关问题：
* \*args与\*\*kwargs之间的关系和区别？



