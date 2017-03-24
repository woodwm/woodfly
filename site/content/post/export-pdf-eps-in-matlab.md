+++
title = "Matlab作图生成pdf, eps，插入Latex"
date = "2017-03-18T17:23:16Z"
tags = ""
categories = ""
slug = "plotting-with-matlab"
+++
对于使用Latex和Matlab的人来说，经常需要面对一个问题，如果保存Matlab的图片，并插入到Latex中。最好选择矢量图形格式，如果用Latex渲染，就用eps格式，用pdflatex渲染，就用pdf格式。

在Matlab的作图窗口中，直接用save as命令，实际上相当于截屏，生成的eps、pdf文件比例不对，而且会产生不必要的边距。

最简单的方式是使用[Export_fig](http://www.mathworks.com/matlabcentral/fileexchange/23629-exportfig)工具箱，能够完美解决这个问题，如果需要保存pdf格式，则需要另外安装ghostscript。

参考：

[What is the best way to include Matlab graphics?](http://tex.stackexchange.com/questions/3995/what-is-the-best-way-to-include-matlab-graphics)

[How to avoid large margins around Matlab plot in PDF](http://tex.stackexchange.com/questions/5559/how-to-avoid-large-margins-around-matlab-plot-in-pdf)
