+++
categories = []
date = "2018-08-24T03:24:37+01:00"
slug = ""
tags = []
title = "Julia-utilies"
type = "post"
+++

## Install packages

### PyCall

Add the path of python in this computer to avoid downloading MiniConda automatically by `Conda.jl`

    ENV["JUPYTER"]="C:\Users\(your_user_name)\AppData\Local\Anaconda3\python.exe"

### IJulia.jl

Use `where jupyter` in the Anaconda cmd to show the path of jupyter. Then set the path of jupyter for IJulia.

    ENV["JUPYTER"]="C:\Users\(your_user_name)\AppData\Local\Anaconda3\Scripts\jupyter.exe"