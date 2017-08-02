+++
categories = []
date = "2017-08-02T16:06:50+00:00"
slug = ""
tags = []
title = "Latex相关"

+++
Latex相关的代码块，一不小心就容易忘掉，虽然还是能通过搜索找到合适的解决方法，还是自己总结一下自己常用的比较好。

# 1. 
![](/uploads/2017/08/02/K7prR.png)

{{ % highlight latex %}}
\documentclass{article}
\usepackage{subcaption}
\usepackage{graphicx}

\begin{document}

\begin{figure}
  \begin{subfigure}{\linewidth}
  \includegraphics[width=.3\linewidth]{example-image-a}\hfill
  \includegraphics[width=.3\linewidth]{example-image-a}\hfill
  \includegraphics[width=.3\linewidth]{example-image-a}
  \caption{}
  \end{subfigure}\par\medskip
  \begin{subfigure}{\linewidth}
  \includegraphics[width=.3\linewidth]{example-image-b}\hfill
  \includegraphics[width=.3\linewidth]{example-image-b}\hfill
  \includegraphics[width=.3\linewidth]{example-image-b}
  \caption{}
  \end{subfigure}\par\medskip
  \begin{subfigure}{\linewidth}
  \includegraphics[width=.3\linewidth]{example-image-c}\hfill
  \includegraphics[width=.3\linewidth]{example-image-c}\hfill
  \includegraphics[width=.3\linewidth]{example-image-c}
  \caption{}
  \end{subfigure}
  \caption{Some grouped images}
\end{figure}

\end{document}
{{ % /highlight %}}