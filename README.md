# 记录我的毕设论文写作时遇到的一些坑

## 1. 字体,STXingkai错误

安装华文行楷字体即可解决

## 2. 任务书中数量只能和模板一致

修改buaathesis.cls中对应函数即可

## 3. misc格式的bibtex参考文献

吧文章类型从@misc改成@other即可

## 4. 参考文献最多写9个

这是latex限制函数最多9个参数导致
可以参考我的方法,自己定义了两个函数,用来处理9个以后的情况

## 5. 插图

```
\begin{figure}[h!] % [h!] 表示尽量排在当前位置
    \centering
    \includegraphics[width=200bp]{figure/pic/model-driving-software-porting.png}
    \caption{模型驱动工程的方法进行源代码移植}
    \label{fig-sample}
\end{figure}
```

## 5. 黑体

黑体的命令是`{\heiti XXX } ` 而不是 `\heite{XXX}`

单独插一张图的时候，width必须是具体长度，而不能用`width=0.35\textwidth`这种等于正文宽度百分比的方法设定





# 感谢

# BUAAthesis[https://github.com/BHOSC/BUAAthesis]

北航毕设论文LaTeX模板