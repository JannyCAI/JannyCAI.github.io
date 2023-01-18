---
title: Latex
updated: '2023-01-18 11:10:10'
excerpt: >-
  latex简介textex是高德纳（donaldeknuth）为排版文字和数学公式而开发的软件。年正在编写《计算机程序设计艺术》的高德纳意识到每况愈下的排版质量将影响其著作的发行为扭转这种状况他着手开发tex发掘当时刚刚用于出版工业的数字印刷设备的潜力。年高德纳发布tex排版引擎而后在年又为更好地支持bit字符和多语言排版而予以改进。tex以其卓越的稳定性跨平台能力和几乎没有bug的特性而著称。它的版本号不断趋近于π当前为。latexlatex​是一种使用tex程序作为排版引擎的​格式（format）可以
tags: []
categories: []
permalink: /post/latex-z1kni9e.html
comments: true
---

# Latex

## 简介

### 1、TeX

**TeX** 是高德纳（Donald E. Knuth）为排版文字和数学公式而开发的软件。1977 年，正在  
编写《计算机程序设计艺术》的高德纳意识到每况愈下的排版质量将影响其著作的发行，为扭转这种状况，他着手开发 TeX，发掘当时刚刚用于出版工业的数字印刷设备的潜力。1982 年，高德纳发布 TeX 排版引擎，而后在 1989 年又为更好地支持 8-bit 字符和多语言排版而予以改进。TeX 以其卓越的稳定性、跨平台能力和几乎没有 bug 的特性而著称。它的版本号不断趋近于 π，当前为 3.141592653。

### 2、LaTeX

**LaTeX**​ 是一种使用 TeX 程序作为排版引擎的 ​**格式**（format），可以粗略地将它理解成是对 TeX 的一层封装。「​**格式**​」定义了一组命令的代码集，高德纳本人还编写了一个简单的 **plain TeX** 格式，而 **LaTeX** 则是当今应用最广泛的 TeX 格式。

LaTeX 由美国计算机科学家莱斯利·兰伯特（Leslie Lamport）在 20 世纪 80 年代初期开发，利用这种格式系统的处理，即使用户没有排版和程序设计的知识也可以充分发挥由 TeX 所提供的强大功能，不必一一亲自去设计或校对，能在几天，甚至几小时内生成很多具有书籍质量的印刷品。对于生成复杂表格和数学公式，这一点表现得尤为突出。

因此它非常适用于生成高印刷质量的科技和数学、物理文档。这个系统同样适用于生成从简单的信件到完整书籍的所有其他种类的文档。

正是因为这些原因，理工科的论文编写，基本是强制使用 LaTeX，而不会用 Word 来编写。

### 3、排版引擎

​**排版引擎**​，是编译源代码并生成文档的程序，如 pdfTeX、XeTeX 和 LuaTeX 等。有时也称其为 **编译器**​。

如果我们将 plain TeX 与 LaTeX 的关系比作 C 和 C++ 的关系，那么 pdfTeX、XeTeX 和 LuaTeX 之间的关系就可以比作是 GCC、LLVM 和 Clang 之间的关系。

* ​**pdfTeX**​：直接生成 PDF，支持 micro-typography；
* ​**XeTeX**​：支持 Unicode、OpenType 与复杂文字编排（CTL），支持中文；
* ​**LuaTeX**​：支持 Unicode、OpenType，内联 Lua，支持中文。

## 主流使用方法

### 在线

​![](assets/net-img-20220407155429-20230115163418-grosvkv.png)​

在本地安装 LaTeX 开发环境是一个字面意义上的「大工程」。不仅配置起来繁琐，而且占用空间极大，大约在 3 到 5 GiB 左右。

所以如果你只是想简单学习一下 LaTeX，可以选择 **Overleaf** 这类云端服务。这类云端服务的好处是有着完整的 LaTeX 环境，并且模板丰富，用户支持好。

[Overleaf, Online LaTeX Editorhttps://www.overleaf.com/](https://www.overleaf.com/)

但是 Overleaf 也有着一定的缺点，例如因为是国外的网站，国内用户在注册及使用的时候可能会碰到网络问题。部分大学也会搭建自己的 Overleaf 版本，例如南京大学的 [在线 LaTeX](https://tex.nju.edu.cn/).

另外的缺点是，Overleaf 的编辑器使用体验并不佳，自动补全等功能也都仅仅是「可用」的程度，远远达不到「好用」的标准。

使用本地的 VS Code 并配上 HyperSnips 等插件，可以让 LaTeX 数学公式的输入速度和准确率上升一个台阶。

‍

### 本地

#### 1、TeX 发行版（distribution）

一个 TeX 发行版是 TeX 排版引擎、支持排版的文件（基本格式、LaTeX 宏包、字体等）以及一些辅助工具的集合。

各式各样的 TeX 发行版经过十多年的发展，大浪淘沙，现今的两个主流发行版为：

* **TeX Live** 由类 UNIX 系统上的 teTeX 发展并取而代之，最终成为「跨平台」的 TeX 发行版。TeX Live 自 2011 年起以年份作为发行版的版本号，保持了一年一更的频率。**MacTeX** 是 macOS（OS X）系统下的一个定制化的 TeX Live 版本，与 TeX Live 同步更新。
* **MiKTeX** 是主要用于 Windows 平台的一个稳定发展的 TeX 发行版，和 TeX Live 相比，它只会安装用得到的宏包，所以体积较小。在中国大陆曾经发行过“CTeX 套装”，它是一个经过本地化配置的 MiKTeX，不过其配置较为过时，也不再有更新支持，使用起来可能有诸多问题，现已不推荐使用。

TeX Live 和 MiKTeX 都集成了一个简单的 LaTeX 源代码编辑器 ​**TeXworks**​（MacTeX 则集成了类似的 ​**TeXShop**​）。用户在安装完毕后，可直接使用 TeXworks 编写和编译 LaTeX 源代码。但是我并不推荐使用这两个源代码编辑器，我们会在下文提到如何使用 **VS Code** 作为编辑器编写 LaTeX。

我们推荐将 ​**TeX Live**、**XeTeX**​ 和 ​**VS Code**​ 作为 LaTeX 本地安装的选择，下文的安装指南均以其为标准。

#### 2、Windows 10 系统

在 Windows 10 下安装 TeX Live，推荐使用「​**镜像安装**​」的方式。

你可以在类似 **南京大学镜像站** 的镜像站，

[NJU Mirrorhttps://mirrors.nju.edu.cn/CTAN/systems/texlive/Images/](https://mirrors.nju.edu.cn/CTAN/systems/texlive/Images/)

下载一个「巨大无比」的安装镜像，即 [texlive2022.iso 文件](https://mirrors.nju.edu.cn/CTAN/systems/texlive/Images/texlive2022-20220321.iso)

双击打开下载的 ISO 文件，Windows 会自动挂载到虚拟光驱，然后弹出一个新的文件夹窗口。如果你安装了一些其他的压缩软件的话，ISO 文件也可能被当成了压缩文件，这时候你就需要将其「​**完整解压**​」到一个「​**不含中文**​」的文件夹下面。

然后，右键菜单，选择「​**以管理员身份运行**​」`install-tl-windows.bat`​ 文件，稍等片刻，便会显示出一个窗口。

​![](assets/net-img-20220407165944-20230115163418-ri5dssk.png)​

保持默认配置，或者设置「不安装 TeXworks 编辑器」，然后安装即可。安装耗时较久，大概在半个小时左右，请耐心等待。

#### 3、Ubuntu 系统

Ubuntu 系统可以通过 `apt`​ 包管理器安装，即可以安装完整版的 TeX Live，也可以只安装自己需要的部分。

* 安装完整版 TeX Live

|

```
sudo apt install texlive-fu
```

||
| --|

* 安装部分 TeX Live（XeTeX + 中文支持 + Science 相关宏包）

|

```
sudo apt install texlive-xetex
sudo apt install texlive-lang-cjk
sudo apt install texlive-science
```

||
| --|

如果一切正常的话，这样就安装完毕了。

## LaTex语法

#### 1、LaTeX 源代码结构

LaTeX 源代码以一个 `\documentclass`​ 命令作为开头，它指定了文档使用的 ​**文档类**​。`\begin{document}...\end{document}`​ 环境当中的内容是文档正文。

在 `\documentclass`​ 和 `\begin{document}`​ 之间的位置称为 ​**导言区**​。在导言区中常会使用 `\usepackage`​ 命令调用宏包，还会进行文档的全局设置，例如设置页面大小、页眉页脚样式、章节标题样式等等。

接在 `%`​ 符号后面的内容是 ​**注释**​，它不会在文档中被渲染出来。如果你想在文档中显示出 `%`​ 这个字符，可以在前面加 ​**反斜杠**​，也就是 `\%`​。

以 **反斜杠** 开头，以第一个 **空格或非字母** 字符结束的一串文字，被称为 ​**控制序列**​，也可以称为 **命令** 或 ​**标记**​，请注意命令是 **区分大小写** 的。

|

```
\documentclass{...} % ... 为某文档类
% 导言区
\begin{document}
% 正文内容
\end{document}
% 此后内容会被忽略
```

||
| --|

#### 2、文档类

一个最简单的英文文档是使用了 `\documentclass{article}`​ 文档类的 latex 源码。

|

```
\documentclass{article}
\begin{document}
``Hello world!'' from \LaTeX.
\end{document}
```

||
| --|

一个最简单的中文文档是使用了 `\documentclass[UTF8]{ctexart}`​ 文档类的 latex 源码。

|

```
\documentclass[UTF8]{ctexart}
\begin{document}
“你好，世界！”来自 \LaTeX{} 的问候。
\end{document}
```

||
| --|

其中 `[UTF8]`​ 是 ​**文档可选参数**​，用以全局规定一些排版参数。

另外的例子是，`[11pt,twoside,a4paper]`​ 指定纸张为 A4 大小，基本字号为 11pt，双面  
排版。

更多相关参数可以参考后面的 ​**扩展阅读**​。

#### 3、宏包

在使用 LaTeX 时，时常需要依赖一些扩展来增强或补充 LaTeX 的功能，比如排版复杂的表  
格、插入图片、增加颜色甚至超链接等等。这些扩展称为宏包。

调用宏包的方法非常类似调用文档类的方法：

|

```
\usepackage[⟨options⟩]{⟨package-name⟩}
```

||
| --|

一些常见的宏包有：

​![](assets/net-img-20220407211116-20230115163419-6mrubk4.png)​

内容来自 [latex-talk](https://github.com/stone-zeng/latex-talk)。

#### 4、谋篇布局

一篇经典的包含各级标题的文章的结构就像这样。

|

```
\documentclass[UTF8]{ctexart}

% 导言区，只是定义一些信息，不会被渲染
\title{你好，world!}  % 标题
\author{Liam}  % 作者
\date{\today}  % 时间设为今天

% 正文内容
\begin{document}

\maketitle  % 渲染标题、作者和时间等信息
\tableofcontents  % 目录

% 各级标题和内容
\section{你好中国}
中国在East Asia.

\subsection{Hello Beijing}
北京是capital of China.

\subsubsection{Hello Dongcheng District}

\paragraph{Tian'anmen Square}
is in the center of Beijing

\subparagraph{Chairman Mao}
is in the center of 天安门广场。

\subsection{Hello 山东}

\paragraph{山东大学} is one of the best university in 山东。

\end{document}
```

||
| --|

我们也可以使用 `\include`​ 之类的命令进行 ​**分文档编译**​。

|

```
\documentclass{book}
% 导言区，加载宏包和各项设置，包括参考文献、索引等
\usepackage{makeidx} % 调用 makeidx 宏包，用来处理索引
\makeindex % 开启索引的收集
\bibliographystyle{plain} % 指定参考文献样式为 plain
\begin{document}
\frontmatter % 前言部分
\maketitle % 标题页
\include{preface} % 前言章节 preface.tex
\tableofcontents
\mainmatter % 正文部分
\include{chapter1} % 第一章 chapter1.tex
\include{chapter2} % 第二章 chapter2.tex
...
\appendix % 附录
\include{appendixA} % 附录 A appendixA.tex
...
\backmatter % 后记部分
\include{epilogue} % 后记 epilogue.tex
\bibliography{books} % 利用 BibTeX 工具从数据库文件 books.bib 生成参考文献
\printindex % 利用 makeindex 工具生成索引
\end{document}
```

||
| --|

#### 5、文本标记

你可以使用一些特定的命令进行文本标记。

* 加粗：`{\bfseries ...}`​ 或 `\textbf{...}`​
* 倾斜：`{\itshape ...}`​ 或 `\textit{...}`​
* 字号：`\tiny`​、`\small`​、`\large`​、`\Large`​ 等
* 换行：`\\`​
* 缩进：`\indent`​
* 居中：`\centering`​ 或 `center`​ 环境

但是，我们 **非常不推荐** 这么做。

还记得吗？我们使用 LaTeX 进行排版的理念是「样式与内容分离」。使用上面这些含有固定含义的文本标记实际上就 **破坏** 了这种理念。

正确合理的做法有以下这些。

* 强调文字（意大利体）：`\emph{...}`​
* 摘要（居中，小字号，带有标题）：`abstract`​ 环境
* 引用（左右边距较大）：`quote`​ 或 `quotation`​ 环境
* 自定义新的命令、环境：`\newcommand\keyword[1]{\textbf{#1}}`​

#### 6、常用环境

列表和枚举：

|

```
\begin{enumerate}
  \item Da Vinci
        \begin{itemize}
          \item \textit{The Last Supper}
          \item \textit{Salvator Mundi}
          \item \textit{Mona Lisa}
        \end{itemize}
  \item Shakespeare
        \begin{itemize}
          \item \textit{Macbeth}
          \item \textit{Hamlet}
          \item \textit{King Lear}
          \item \textit{Othello}
        \end{itemize}
\end{enumerate}
```

||
| --|

图片：

|

```
% 不是 graphics，放到导言区
\usepackage{graphicx}
% 可以统一指定图片路径
\graphicspath{{./images/}}

\begin{figure}
  \centering
  % 可指定宽度、高度等选项
  \includegraphics[...]{fudan-logo.pdf}
  \caption{Logo of Fudan University}
  \label{fig:fudan-logo}
\end{figure}
```

||
| --|

表格：

|

```
\usepackage{booktabs}  % 三线表
\begin{table}
  \caption{Population Census of China}
  \label{tab:china-population}
  % 列格式：c 居中，l 左对齐，r 右对齐
  \begin{tabular}{cc}
    \toprule
    Year     & Population \\
    \midrule
    1953     & 6.0        \\
    ... 2020 & 14.1       \\
    \bottomrule
  \end{tabular}
\end{table}
```

||
| --|

定理：

|

```
\usepackage{amsthm}
% 需要预先定义
\newtheorem{theorem}{Theorem}
\newtheorem*{remark}{Remark}  % 不编号

\begin{theorem}[Fermat]
  $a^n+b^n=c^n$ has no positive...
\end{theorem}
\begin{proof}
  % 证明后面会有 QED 符号 
  It's obvious.
\end{proof}
\begin{remark}
  The cases $n=1$ and $n=2$...
\end{remark}
```

||
| --|

语法高亮：

|

```
\usepackage{listings}
\usepackage{xcolor}
\lstset{
    columns=fixed,     
    numbers=left,                                        % 在左侧显示行号
    frame=none,                                          % 不显示背景边框
    backgroundcolor=\color[RGB]{245,245,244},            % 设定背景颜色
    keywordstyle=\color[RGB]{40,40,255},                 % 设定关键字颜色
    numberstyle=\footnotesize\color{darkgray},           % 设定行号格式
    commentstyle=\it\color[RGB]{0,96,96},                % 设置代码注释的格式
    stringstyle=\rmfamily\slshape\color[RGB]{128,0,0},   % 设置字符串格式
    showstringspaces=false,                              % 不显示字符串中的空格
    language=c++,                                        % 设置语言
}

% 引入文件的写法
% \lstinputlisting[language=c++]{main.cpp}
% 直接写法
\begin{lstlisting}
  #include <iostream>
  int main()
  {
      std::cout << "Hello, World!" << std::endl;
  }  
\end{lstlisting}
```

||
| --|

‍

‍

‍

‍

## LaTex VS Code 环境配置

VS Code 及 LaTeX Workshop 插件安装

安装 VS Code 的方式已经在之前的博文中讲过了，可以去 [官网](https://code.visualstudio.com/Download) 下载。

然后是安装 LaTeX Workshop 插件，在打开 VS Code 之后，点左侧的插件商店选项，搜索 `LaTeX Workshop`​，然后安装即可。

​![](assets/net-img-20220407172801-20230115163419-hkav6mv.png)​

安装完成后，新建一个 `.tex`​ 文件，将以下内容复制进去，然后保存。

|

```
\documentclass{ctexart}
\begin{document}
你好，\LaTeX{}!
\end{document}
```

||
| --|

接着点击左侧 TeX 面板的 `Build LaTeX`​ 和 `View LaTeX PDF`​ 即可。

​![](assets/net-img-20220407172453-20230115163419-9vkl8ki.png)​

‍

‍

‍

‍

‍

## LaTeX数学公式

### 前言

[第 5 期、写作：LaTeX 和 Markdown 中的数学公式和 HyperSnips 快捷输入 | OrangeX4&apos;s Blog](https://orangex4.cool/post/lesson-zero-5/#:~:text=KaTeX%20%EF%BC%9A%20%E5%B0%8F%E8%80%8C%E5%BF%AB%20%E7%9A%84%E6%95%B0%E5%AD%A6%E5%85%AC%E5%BC%8F%E6%B8%B2%E6%9F%93%E5%BA%93%E3%80%82%20%E5%9B%A0%E4%B8%BA%20KaTeX%20%E5%B0%86%E6%B3%A8%E6%84%8F%E5%8A%9B%E5%AE%8C%E5%85%A8%E6%8A%95%E5%85%A5%E4%BA%8E%E5%B0%86%20%E6%A0%87%E5%87%86,physics%20%E5%AE%8F%E5%8C%85%EF%BC%8C%E4%B9%9F%E4%B8%8D%E6%89%93%E7%AE%97%E5%B0%86%E5%85%B6%E6%B8%B2%E6%9F%93%E6%88%90%20SVG%20%E7%AD%89%E5%9B%BE%E5%BD%A2%EF%BC%8C%E6%89%80%E4%BB%A5%E6%B8%B2%E6%9F%93%E9%80%9F%E5%BA%A6%E6%9E%81%E5%BF%AB%E3%80%82%20MathJax%20%EF%BC%9A%20%E5%A4%A7%E8%80%8C%E5%85%A8%20%E7%9A%84%E6%95%B0%E5%AD%A6%E5%85%AC%E5%BC%8F%E6%B8%B2%E6%9F%93%E5%BA%93%E3%80%82)

书写「​**数学公式**​」一直都是写作中的一个难点，使用 Word 之类的软件的时候，往往需要类似 MathType 之类的第三方插件来帮助输入，而且输入效率低下。

如今编写数学公式，「​**LaTeX 式数学公式**​」已经成为了事实标准，无论是 LaTeX 自身，还是 Markdown，甚至是 Word 里面的使用的 MathType 和 AxMath，事实上都支持 LaTeX 式的语法，其特点是类似 `\int_a^b xdx`​ 这样，特殊符号使用以 **反斜杠** 开头的 **命令** 来表示。

然而，直接使用 LaTeX 式的语法来写，输入效率依然很差。

但是在使用了 **VS Code**​ 和 ​**Markdown**，以及一些 **VS Code 插件** 之后，输入效率会 **大幅提升**，甚至能达到比手写更快的效果。

### 数学公式主流方法

#### 1. word流

初学者刚开始学习如何编辑数学公式时，很容易就会碰到这两款软件。分别是 [MathType](https://www.mathtype.cn/) 和 [AxMath](https://www.amyxun.com/)，它们均可以内嵌到 Word 里。

​![](assets/net-img-20220408150130-20230115163419-3z6spjs.png)​

* ​**MathType**​：老牌软件，优点是普及率高，使用 Word 编辑数学公式的人基本上都用过 Mathtype，所以兼容性比较好。缺点是界面不美观，使用起来复杂，​**正版价格昂贵**​，年订阅制，且每年要 338 元。
* ​**AxMath**​：新创软件，优点是界面清晰，使用简单，与 LaTeX 数学公式互转效果好。但缺点是普及率低，迁移难度大，如果对方电脑里面没有安装 AxMath，就只能以图片形式展示，而不能编辑。​**正版价格适中**​，买断制，一共 36 元

然而，实际上，如果你编辑数学公式的需求 **比较少**，那么可以直接使用下文会提到的​ ​**在线 LaTeX 数学公式编辑器**[在线LaTeX公式编辑器-编辑器 (latexlive.com)](https://www.latexlive.com/home##)，不仅支持 **可视化操作**，而且 **完全免费**，能够生成 **多种图片格式** 以供内嵌到 Word 文档中。

如果你编辑数学公式的需求 ​**比较多**​，那为什么不花费一两个小时，学习一下 LaTeX 或 Markdown 中数学公式的编辑方法呢？不仅 ​**完全免费**​，而且 ​**方便后续编辑**​，并且使用 VS Code 及插件之后，​**输入效率会高几个数量级**​。

#### 2. Latex 

**LaTeX** 原生支持数学公式，再加上 **amsmath 宏包**，就能以清晰美观的方式编辑数学公式。​#LaTex#​

​![](assets/net-img-20220408152227-20230115163420-suakgbn.png)​

#### 3. 公式识别

当前数学公式识别做得比较好的是 [Mathpix Snip](https://mathpix.com/).

​![](assets/net-img-20220408155910-20230115163420-vneqeb5.png)​

[Mathpix Sniphttps://mathpix.com/](https://mathpix.com/)

Mathpix Snip 有着 ​**超高的识别精准度**​，甚至能够精准地识别手写的数学公式。

#### 4. Web流

我们当然也有相应的 JS 库来实现 LaTeX 式数学公式在 **网页上** 的 **渲染**，甚至是 **编辑**。当前常见的渲染库有 [KaTeX](https://katex.org/) 和 [MathJax](https://www.mathjax.org/)。 ​#KaTex#​

* ​**KaTeX**​：**小而快** 的数学公式渲染库。因为 KaTeX 将注意力完全投入于将 **标准 LaTeX 数学公式** 渲染成 ​**HTML 元素**​，而不考虑 LaTeX 拓展语法，例如 physics 宏包，也不打算将其渲染成 SVG 等图形，所以渲染速度极快。
* ​**MathJax**​：**大而全** 的数学公式渲染库。可以将以 ​**LaTeX**​、**MathML** 和 **AsciiMath** 语法书写的数学公式，渲染成 ​**HTML**​、**SVG** 或 ​**MathML**​。并且支持扩展，比如 **physics 宏包** 和 ​**amsmath 宏包**​。

**Markdown** 一般就是使用这两个库其中之一来渲染数学公式的。

VS Code 的​ ​**Markdown Preview Enhanced** 可以自由在 KaTex 和 MathJax 之间切换。

博主个人常用的是 **KaTeX**，因为它渲染速度快，而且也支持了博主需要的所有功能。

除了数学渲染，也有支持 **可视化编辑** 的数学公式库，例如 [MathLive](https://cortexjs.io/mathlive/demo/)。

顺便要提到的是一个 **在线 LaTeX 数学公式编辑器**​[LaTeX 公式编辑器https://www.latexlive.com/home##](https://www.latexlive.com/home##)，它是由 UP 主 [妈咪说](https://www.bilibili.com/video/BV14g4y1q7pb) 借助 **MathJax** 和 **Mathpix 接口** 开发的一个在线工具。使用这个在线网站，就可以避免使用 MathType 和 AxMath 这类收费软件了。

### LaTex公式语法

‍

#### 1. 上标和下标

```
上标 $x^2 + y^{12} = 1$

上标 $x_1 + y_{12} = 1$
```

​![](assets/net-img-v2-a527faa78367be526a55992ebfae09f9_720w-20230115163420-ndwatpv.png)​

#### 2. 分式

```
较小的行内行分数 $\frac{1}{2}$

展示型的分式 $\displaystyle\frac{x+1}{x-1}$
```

其中 `\displaystyle`​ 用于将行内展示转为块状展示.

​![](assets/net-img-v2-6068b9817b165318fbb44912601a1450_720w-20230115163420-ef05c6q.png)​

#### 3.根式

```
开平方 $\sqrt{2}$

开 $n$ 次方 $\sqrt[n]{2}$
```

​![](assets/net-img-v2-7f43224f74cae008fa950a82252e0903_720w-20230115163420-4kmfjsg.png)​

#### 4. 空格

数学公式中的 **空格和换行** 都会在编译时 ​**被忽略**​，想要实现「空格」的效果，需要用特别的命令。

```
紧贴 $a\!b$

没有空格 $ab$

小空格 $a\,b$

中等空格 $a\;b$

大空格 $a\ b$

quad 空格 $a\quad b$

两个 quad 空格 $a\qquad b$
```

​![](assets/net-img-v2-3d5d3d55a6cc7fa4108a3d72287ec509_720w-20230115163420-hc3e0hr.png)​

#### 5.累加、累乘和积分

```
累加 $\sum_{k=1}^n\frac{1}{k}  \quad  \displaystyle\sum_{k=1}^n\frac{1}{k}$

累乘 $\prod_{k=1}^n\frac{1}{k}  \quad  \displaystyle\prod_{k=1}^n\frac{1}{k}$

积分 $\displaystyle \int_0^1x{\rm d}x  \quad  \iint_{D_{xy}}  \quad  \iiint_{\Omega_{xyz}}$
```

​![](assets/net-img-v2-107c58a00665db46695c759d10926ded_720w-20230115163420-aligodp.png)​

#### 6. 括号修饰

用 `\left`​ 和 `\right`​ 可以让括号适配内部大小

```
圆括号 $\displaystyle \left(\sum_{k=1}^{n}\frac{1}{k} \right)^2$

方括号 $\displaystyle \left[\sum_{k=1}^{n}\frac{1}{k} \right]^2$

花括号 $\displaystyle \left\{\sum_{k=1}^{n}\frac{1}{k} \right\}^2$

尖括号 $\displaystyle \left\langle\sum_{k=1}^{n}\frac{1}{k} \right\rangle^2$
```

​![](assets/net-img-v2-2564e223b37d79424ff60ecf1ee4e5b6_720w-20230115164228-d69k6re.png)​

‍

#### 7. 多行算式对齐

```
居中:

$$
\begin{aligned}
y &=(x+5)^2-(x+1)^2 \\
&=(x^2+10x+25)-(x^2+2x+1) \\
&=8x+24 \\
\end{aligned}
$$

左对齐:

$
\begin{aligned}
y &=(x+5)^2-(x+1)^2 \\
&=(x^2+10x+25)-(x^2+2x+1) \\
&=8x+24 \\
\end{aligned}
$
```

​![](assets/net-img-v2-2ce4065baebaa934da5963574f65bce7_720w-20230115164229-2s1u2fz.png)​

‍

#### 8. 方程组

```
$$
\begin{cases}
k_{11}x_1+k_{12}x_2+\cdots+k_{1n}x_n=b_1 \\
k_{21}x_1+k_{22}x_2+\cdots+k_{2n}x_n=b_2 \\
\cdots \\
k_{n1}x_1+k_{n2}x_2+\cdots+k_{nn}x_n=b_n \\
\end{cases}
$$
```

​![](assets/net-img-v2-a085a39d41c0af5ded6b328907e662ec_720w-20230115164229-gg0pps4.png)​

‍

#### 9. 矩阵

```
矩阵:

$$
\begin{pmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{pmatrix}

\quad

\begin{bmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{bmatrix}
$$ 

行列式: 

$$
\begin{vmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{vmatrix}
$$
```

​![](assets/net-img-v2-8f249643b32b0fd0375dc8f8c8b40d86_720w-20230115164229-8m4mmhz.png)​

‍

#### 10. 特殊字符

​![](assets/net-img-v2-842b02c54dd7d8e0571609414e79bdc1_720w-20230115164232-17fkg2t.png)​

更多特殊符号可以 [上网查询](https://oeis.org/wiki/List_of_LaTeX_mathematical_symbols)

可以搜索 “Latex 符号表

#### 11. 公式编号与引用

```
$$
x+2 \tag{1.2}
$$

$$
\begin{equation}
x^n+y^n=z^n
\end{equation}
$$

由公式 $(1.2)$ 可得到结论
```

​![](assets/net-img-v2-e602d10556b445efba976af2ee0b4209_720w-20230115164234-aeqfvwt.jpg)​

#### 12. 零碎的重要语法

* 点乘 `$\cdot$`​, 叉乘 `$\times$`​, 异或 `$\otimes$`​, 直和 `$\oplus$`​, 加减 `$\pm$`​, 复合 `$\circ$`​.
* 小于等于 `$\leq$`​, 大于等于 `$\geq$`​, 不等 `$\neq$`​, 恒等 `$\equiv$`​, 约等 `$\approx$`​, 等价 `$\cong$`​, 相似 `$\sim$`​, 相似等于 `$\simeq$`​, 点等 `$\doteq$`​.
* 逻辑与 `$\land$`​, 逻辑或 `$\lor$`​, 逻辑非 `$\lnot$`​, 蕴涵 `$\to$`​, 等价 `$\leftrightarrow$`​.
* 因为 `$\because$`​, 所以 `$\therefore$`​, 存在 `$\exist$`​, 任意 `$\forall$`​.
* 左小箭头 `$\leftarrow$`​, 右小箭头 `$\rightarrow$`​, 左大箭头 `$\Leftarrow$`​, 右大箭头 `$\Rightarrow$`​, 右长箭头 `$\xrightarrow[fgh]{abcde}$`​.
* 属于 `$\in$`​, 包含于 `$\subset$`​, 真包含于 `$\subseteq$`​, 交 `$\cap$`​, 并 `$\cup$`​, 空集 `$\empty$`​
* 短向量 `$\vec{x}$`​, 长向量 `$\overrightarrow{AB}$`​, 上横线 `$\overline{p}$`​.
* 无限 `$\infty$`​, 极限 `$\lim$`​, 微分 `${\rm d}$`​, 偏导 `$\partial$`​, 点求导 `$\dot{y}$`​, 点二阶导 `$\ddot{y}$`​, 变化量 `$\Delta$`​, 梯度 `$\nabla$`​.
* 横省略 `$\cdots$`​, 竖省略 `$\vdots$`​, 斜省略 `$\ddots$`​.
* 常见函数 `$\sin$`​, `$\cos$`​, `$\tan$`​, `$\arcsin$`​, `$\arccos$`​, `$\arctan$`​, `$\ln$`​, `$\log$`​, `$\exp$`​.

​![](assets/net-img-v2-1063f781baa2bed9e7ebb32428719650_720w-20230115164235-obf4e35.png)​

还有特别重要的数集、向量、矩阵符号：

```
RR  =>  \mathbb{R}
NN  =>   \mathbb{N}
txt  =>  \text{...}
xbar  =>  \bar{x}
xhat  =>  \hat{x}
xhvec  =>  \vec{x}
xhdot  =>  \dot{x}
Xbb  =>  \mathbb{X}
Xbs  =>  \boldsymbol{X}
Xbm  =>  \bm{X}
Xbf  =>  \mathbf{X}
Xsf  =>  \mathsf{X}
Xcal  =>  \mathcal{X}
Xfrak  =>  \mathfrak{X}
Xrm  =>  \mathrm{X}
```

#### ⭐**注意：不要在公式内写中文**

‍

‍

### 数学公式VS Code环境配置

如何使用 VS Code 编辑 Markdown 或 LaTeX 中的数学公式

默认你安装好了 **VS Code** 和 **Markdown Preview Enhanced** 插件。

‍

‍

## 服务器 Overleaf 部署指南

	本地 vscode  的编译器五花八门琳琅满目，配置也极其复杂和不统一。发现了 Overleaf 这个all-in-one 网站，这个程序是开源的，可以部署到自己的服务器上。可以愉快地写 LaTeX 啦！

	Overleaf 在 Github 上的项目地址在[这里](https://github.com/overleaf/overleaf)。由于直接提供了 Docker，所以安装过程非常简单。

‍

‍

‍

‍

‍

‍

## 参考资料

### LaTex相关

#### 资料

1. 便携式文档格式 - Wikipedia - [https://zh.wikipedia.org/wiki/可移植文档格式](https://zh.wikipedia.org/wiki/%E5%8F%AF%E7%A7%BB%E6%A4%8D%E6%96%87%E6%A1%A3%E6%A0%BC%E5%BC%8F)
2. LaTeX - Wikipedia - [https://zh.wikipedia.org/wiki/LaTeX](https://zh.wikipedia.org/wiki/LaTeX)
3. 呈现与内容分离 - Wikipedia - [https://zh.wikipedia.org/wiki/呈现与内容分离](https://zh.wikipedia.org/wiki/%E5%91%88%E7%8E%B0%E4%B8%8E%E5%86%85%E5%AE%B9%E5%88%86%E7%A6%BB)
4. Microsoft Word - Wikipedia - [https://zh.wikipedia.org/wiki/Microsoft_Word](https://zh.wikipedia.org/wiki/Microsoft_Word)
5. amsmath 包使用手册 - [http://static.latexstudio.net/article/2019/0204/amsmath-guide-zh-cn.pdf](http://static.latexstudio.net/article/2019/0204/amsmath-guide-zh-cn.pdf)
6. Documentation - Overleaf, Online LaTeX Editor - [https://www.overleaf.com/learn](https://www.overleaf.com/learn)
7. 一份其实很短的 LaTeX 入门文档 - [https://liam.page/2014/09/08/latex-introduction/](https://liam.page/2014/09/08/latex-introduction/)
8. 在 Ubuntu 中安装 TEX Live 2018 - [https://stone-zeng.github.io/2018-05-13-install-texlive-ubuntu/](https://stone-zeng.github.io/2018-05-13-install-texlive-ubuntu/)
9. 一份（不太）简短的 LATEX 2ε 介绍 - [https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/](https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/)
10. 当代 TeX 发行版超快速安装指南 - [https://git.nju.edu.cn/atXYblip/install-latex-instantly](https://git.nju.edu.cn/atXYblip/install-latex-instantly)
11. 一份简短的关于 LaTeX 安装的介绍 - [https://mirrors.mit.edu/CTAN/info/install-latex-guide-zh-cn/install-latex-guide-zh-cn.pdf](https://mirrors.mit.edu/CTAN/info/install-latex-guide-zh-cn/install-latex-guide-zh-cn.pdf)
12. LaTeX 之代码语法高亮 - [https://www.latexstudio.net/archives/5900.html](https://www.latexstudio.net/archives/5900.html)
13. 现代 LaTeX 入门讲座 - [https://github.com/stone-zeng/latex-talk](https://github.com/stone-zeng/latex-talk)

#### 延展阅读

[曾祥东](https://github.com/stone-zeng/latex-talk) 的「现代 LaTeX 入门讲座」，十分推荐大家看一看。

[现代 LaTeX 入门讲座https://github.com/stone-zeng/latex-talk](https://github.com/stone-zeng/latex-talk)

简易的 TeX 发行版安装指南。

[当代 TeX 发行版超快速安装指南https://git.nju.edu.cn/atXYblip/install-latex-instantly](https://git.nju.edu.cn/atXYblip/install-latex-instantly)

详细的 LaTeX 安装介绍。

[一份简短的关于 LaTeX 安装的介绍https://mirrors.mit.edu/CTAN/info/install-latex-guide-zh-cn/install-latex-guide-zh-cn.pdf](https://mirrors.mit.edu/CTAN/info/install-latex-guide-zh-cn/install-latex-guide-zh-cn.pdf)

一份十分详尽的 LaTeX 2 介绍。

[一份（不太）简短的 LATEX 2ε 介绍https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/lshort-zh-cn.pdf](https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/lshort-zh-cn.pdf)

更详细的文档也可以看看 Overleaf 家的文档（英文）。

[Documentation - Overleaf, Online LaTeX Editorhttps://www.overleaf.com/learn](https://www.overleaf.com/learn)

### LaTex数学公式相关

#### 资料

1. 一份（不太）简短的 LATEX 2ε 介绍 - [https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/](https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/)
2. LaTeX/Mathematics - [https://en.wikibooks.org/wiki/LaTeX/Mathematics](https://en.wikibooks.org/wiki/LaTeX/Mathematics)
3. Mathematical expressions - Overleaf, Online LaTeX Editor - [https://www.overleaf.com/learn/latex/Mathematical_expressions](https://www.overleaf.com/learn/latex/Mathematical_expressions)
4. 怎么在 Word 中方便地输入数学公式？- [https://www.zhihu.com/question/24613226](https://www.zhihu.com/question/24613226)
5. Axmath和Mathtype主要有什么区别？为什么Mathtype卖的那么贵？- [https://www.zhihu.com/question/55740822](https://www.zhihu.com/question/55740822)
6. MathType - [https://www.mathtype.cn/](https://www.mathtype.cn/)
7. AxMath - [https://www.amyxun.com/](https://www.amyxun.com/)
8. KaTeX - [https://katex.org/](https://katex.org/)
9. MathJax - [https://www.mathjax.org/](https://www.mathjax.org/)
10. Math Live - [https://cortexjs.io/mathlive/demo/](https://cortexjs.io/mathlive/demo/)
11. LaTeX 公式编辑器 - [https://www.latexlive.com/home##](https://www.latexlive.com/home##)
12. Mathpix - [https://mathpix.com/](https://mathpix.com/)
13. OrangeX4’s HyperSnips - [https://github.com/OrangeX4/OrangeX4-HyperSnips/blob/main/markdown.hsnips](https://github.com/OrangeX4/OrangeX4-HyperSnips/blob/main/markdown.hsnips)
14. HyperSnips - [https://github.com/draivin/hsnips](https://github.com/draivin/hsnips)

#### 延展阅读

一份十分详尽的 LaTeX 2 介绍。

[一份（不太）简短的 LATEX 2ε 介绍https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/lshort-zh-cn.pdf](https://github.com/CTeX-org/lshort-zh-cn/releases/download/v6.03/lshort-zh-cn.pdf)

Wiki Book 上有关的介绍（英文）。

[LaTeX/Mathematicshttps://en.wikibooks.org/wiki/LaTeX/Mathematics](https://en.wikibooks.org/wiki/LaTeX/Mathematics)

Overleaf 家数学公式文档（英文）。

[Mathematical expressions - Overleaf, Online LaTeX Editorhttps://www.overleaf.com/learn/latex/Mathematical_expressions](https://www.overleaf.com/learn/latex/Mathematical_expressions)

‍

#### 服务器相关

[服务器 Overleaf 部署指南 - SkyWT](https://blog.skywt.cn/posts/self-host-overleaf)

‍

‍


