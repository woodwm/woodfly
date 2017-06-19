+++
categories = []
date = "2017-06-19T22:24:22+00:00"
slug = "matlab-tricks"
tags = ["Matlab"]
title = "Matlab使用技巧（都是血汗的积累）"

+++
## 1. 动态更改文件名

如，par1 = 1.0，par2 = 2.0，得到的结果为数组arr_t则可设置输出文件名

```matlab
filenm = ['ex_p1_' num2str(par1) '_p2' num2str(par2) '.mat'];
save(filenm,   'arr_t');
```
##