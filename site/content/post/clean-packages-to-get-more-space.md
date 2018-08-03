+++
categories = []
date = "2018-08-03T16:46:44+01:00"
draft = true
slug = "clean-packages"
tags = []
title = "Clean packages to get more space"

+++
## Python

I am happy using `anaconda` and `conda` to manage the python packages. After a long time of usage, there will be many old version packages downloaded and tarballs.

Remove index cache, tarballs, unused cache packages
`conda clean --all`