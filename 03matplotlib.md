# 记录Matplotlib笔记
>## 一、Matplotlib函数总结：
### 1.绘制条形图
[Matplotlib中的颜色、线条、标记样式汇总(感谢知乎大佬-Mr.喵)](https://zhuanlan.zhihu.com/p/40992563)
```python
from matplotlib import pyplot as plt #导入matplotlib文件中的pyplot.py画图模块  (import matplotlib.pyplot as plt)
from matplotlib import font_manager #导入matplotlib文件中的font_manager.py字体管理模块

###########################################创建绘图窗口并绘制图像#############################################
#生成绘图窗口（图像名，图像大小，分辨率）
plt.figure(num="int"or"str",figsize=(float,float), dpi=float)

#
*****fig.suptitle("draw some subplot")****

#生成子绘图窗口（n行，n列，索引）
plt.subplot(nrows, ncols, index)

#
****ax1.set_title("y1 = x")****

#############################################绘制图像（曲线，散点，条形）###########################################
#绘制曲线(横纵坐标，曲线格式，数据点格式，透明度
plt.plot(x, y, color, linestyle, linewidth, marker, markersize, markerfacecolor, alpha)

#绘制散点图(横纵坐标，散点大小，颜色，格式，透明度)
plt.scatter(x, y, s, color, marker, alpha)

#绘制竖状条形图（起始横坐标，起始纵坐标，高度，宽度，颜色，透明度，标签相对条形的位置）
plt.bar(x, bottom, height, width, color, alpha, align='center'or'edge')

#绘制横状条形图（起始纵坐标，起始横坐标，高度，宽度，颜色，透明度，标签相对条形的位置）
plt.barh(y, left, width, height, color, alpha, align='center'or'edge')

****#绘制直方图****


#####################################################对绘图窗口进行操作##############################################
my_font = font_manager.FontProperties(fname="C:\Windows\Fonts\SIMFANG.TTF") #采用系统文件中的中文格式
#设置x轴的刻度（x轴刻度的取值，刻度的字符，刻度的旋转度数，设置中文字体）
plt.xticks(range, _xticks_labels, rotation, FontProperties=my_font)

#对图像添加标题（标题名，格式，旋转角度，透明度，设置中文字体）
plt.title(label, color, fontsize, fontweight, rotation, alpha, FontProperties=my_font)

#设置x轴的名称(名称字符串，位置，设置中文字体)
plt.xlabel(xlabel="x-axes", loc='center', FontProperties=my_font)

#设置x轴的范围
plt.xlim(x_min,x_max)

#添加网格线（网格方向，格式，透明度）
plt.grid(axis='x'or'y'or'both', color, linestyle, linewidth, alpha)

#添加图例（图例名字，位置，字体大小，图例的中文格式，标题名）
plt.legend(labels, loc, fontsize, prop=my_font, title)

#添加水印（水印左下角坐标，水印内容，字体格式，透明度）
plt.text(x, y, s, fontsize, color, alpha)

#保存图像  在plt.show()之前调用plt.savefig(“路径文件名”)  相比jpg，svg放大后不会失真
plt.savefig("fname")

plt.show() #展示图像

```


>## 二、Matplotlib相关问题：
* \*args与\*\*kwargs之间的关系和区别？



