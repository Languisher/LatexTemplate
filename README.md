# LatexTemplate

## SJTUBeamerTemplate

### 初始化设置

个人使用需修改：
```latex 
\title[\SJTUBeamer 示例文档] % 页脚显示标题
{\textbf{如何使用 \LaTeX{} 排版论文}} % 首页标题

\subtitle{\SJTUBeamer 示例文档}
```
### 如何运行

在根文件夹中输入：

```shell
make
open main.pdf
```

### 幻灯片基本操作

SJTUBeamer 对该项目有一个简短的教程，详情请点击[链接](./SJTUBeamerDoc.pdf)

#### 文件架构

```
main.tex 
contents/
|--- introduction 
|--- basis 
|--- summary
```

并在 `main.tex` 文件中在插入位置加入以下代码：
```latex
\include{contents/introduction}
\include{contents/basis}
\include{contents/summary}
```

#### 幻灯片主体结构

插入章节

```latex
\section{content}
\subsection{content}
```

插入新幻灯片

```latex
\begin{frame}{frametitle}
    framecontent
\end{frame}
```

#### 幻灯片内元素



