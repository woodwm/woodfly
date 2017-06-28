+++
categories = []
date = "2017-06-19T22:24:22Z"
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
## 2. 修改循环变量（调试技巧）
Matlab中一旦进入for循环后，无法自行修改循环变量i的值。即使修改了，在下一步循环中，循环变量还是会改回去。

```
for i = 1:3
    i = 1;
end
```
每一步中i的值分别为1,2,3.

## 3. 使用相对地址导入文件
使用`..`表示包含当前文件夹的上一级文件夹，所以`Folder1`是当前文件夹，`Folder2`是当前文件夹的下一级文件夹。

	load(fullfile('..', 'Folder1', 'Folder2', files.name));