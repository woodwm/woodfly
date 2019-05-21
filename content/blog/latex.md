+++
title = "Latex问题和解决方法"
date = "2017-08-02T16:06:50Z"
slug = "latex-codes"
categories = []
tags = []
type = "post"
+++

Latex相关的代码块，一不小心就容易忘掉，虽然还是能通过搜索找到合适的解决方法，还是自己总结一下自己常用的比较好。

# 1. 多个图合并为一个子图
f1   f2   f3
     (a)
f4   f5   f6
     (b)
```
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

```

# 2. 子图排列在不同页

```
\begin{figure}[htb]
    \centering
    \begin{subfigure}[b]{\textwidth}
        \includegraphics[width=0.6\textwidth]{example-image}
        \subcaption{$Q^{*}$ values for arm 1}
        \label{fig:arm1}
    \end{subfigure}
%
    \begin{subfigure}[b]{\textwidth}
        \includegraphics[width=0.6\textwidth]{example-image}
        \subcaption{$Q^{*}$ values for arm 2}
        \label{fig:arm2}
    \end{subfigure}
    \caption{$Q^{*}$ values for different arms}
\end{figure}
\begin{figure}[htb]\ContinuedFloat
    \centering
    \begin{subfigure}[b]{\textwidth}
        \includegraphics[width=0.6\textwidth]{example-image}
        \subcaption{$Q^{*}$ values for arm 3}
        \label{fig:arm3}
    \end{subfigure}
%
    \begin{subfigure}[b]{\textwidth}
        \includegraphics[width=0.6\textwidth]{example-image}
        \subcaption{$Q^{*}$ values for arm 4}
        \label{fig:arm4}
    \end{subfigure}
    \caption{$Q^{*}$ values for different arms (cont.)}
    \label{fig:arms}
\end{figure}
```