+++
title = "Python的一些经验"
date = "2017-09-02T00:46:01Z"
slug = "python-tips"
categories = []
tags = []
type = "post"
+++

## numba不支持`dict`,可用`namedtuples`代替

numba does not support `dict` type. A good way to replace it is using `namedtuples`

```python
import numpy as np
from collections import namedtuple

conf = namedtuple('conf', ['a', 'b', 'c'])
func(conf(1, 2.0, np.array([1,2,3], dtype=np.int64)))
```

## 