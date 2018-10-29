+++
categories = []
date = "2018-10-29T23:25:53+00:00"
draft = true
slug = ""
tags = ["latex"]
title = "use pandoc to convert latex to word"

+++
目前比较好的一种把latex文件转为word文件的方法是使用`pandoc`,

首先安装`pandoc`和`pandoc-citeproc`:

```
brew install pandoc
brew install pandoc-citeproc
```

然后调用`pandoc`：
`pandoc my-document.tex --bibliography=library.bib -o my-document.docx`