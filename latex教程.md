# latex 教程

[toc]

## latex 优势

- 对公式编辑和显示极其友好
- 对交叉引用的支持十分便捷
- 程序员思维，让用户精力集中于内容输出，而不是浪费在格式排版上

## 麻烦？

- 有模板的latex才是生产力
- 找到latex模板

## 软件的安装

- 推荐使用[overleaf]() 在线编辑latex论文，便于跨平台使用，但是需要一直在线。

- 也可以使用本地编辑的方式，推荐**texlive + texstudio**

  

  ---

  

- [texlive | 清华大学开源软件镜像站](https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/)    环境

- [texstudio](https://sourceforge.net/projects/texstudio/)   IDE

  

## 如何写论文

### **章节标题， 一般只需要二级标题**

`\section{}`

`\subsection{}`

`\subsubsection{}`

### **如何分段**

双回车

### **插入图， 表， 公式，**

- 插入图

```
\begin{figure}[H]	
	\includegraphics[width=0.55\textwidth]{../fig/fig-accVSiteration.pdf}
	\caption{title.\label{key})}
\end{figure} 
```

- 插入表格

```
使用excel宏
```

- 插入公式

```
\begin{equation}
    X = WX + b
	\label{key1}
\end{equation}
```

$X = WX + b$  



### **引用图，表，公式**

- 交叉引用

- `\label{key}`

- `\ref{key}`

### **作者信息**

### **如何引用参考文献**

- 使用文献管理工具

- 生成bib文件

  - 期刊：标题，作者，日期，期，卷，期刊名（一般使用缩写），页码
  - 会议：标题，作者，日期，会议举办地点，会议名，页码

- `\cite{key}`，文件尾部需要加入引用命令，直接搜索引擎检索就行

  

### **注释**

### **trick： 所见即所得的修改文章**

---

----

## 进阶

- 如何使用里面的语法检测工具
- 编译生成的文件，简单的介绍

## 如何获取对应期刊的latex模板

- 以 sensors 为例，如何找到对应的latex模板

  


