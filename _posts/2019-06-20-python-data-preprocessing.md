---
title: "Python Learning"
author: "yue"
date: '2019-06-20'
excerpt: "My experiences in learning Python"
layout: post
permalink: /blog/2019/06/python-data-preprocessing/
categories:
  - Data Preprocessing
  - Python
  - SQL
  - Audio Journal Archive
---

## Python Concatenating Columns
```{python}
df.ix[: colnames].astype(str).add('delimiter').sum(axis=1)
```

## Shuffle row indices
```{python}
import numpy as np
np.random.permutation(df.shape[0])
```

## Pad values 
```{python}
import numpy as np
np.repeat([[1, 2],[3, 4]], times)

# returns : array([1, 1, 2, 2, 3, 3, 4, 4]) when times = 2
```
repeat each atomic element in the data structure by the specified number of times

```{python}
np.tile([[1, 2], [3, 4]], times)

# returns :
array([[1, 2, 1, 2],
       [3, 4, 3, 4]]) when times = 2
```
repeat one whole data structure by the specified number of times




[Audio Journal Python Decorator](https://www.youtube.com/watch?v=NkDaYH5xfb0&feature=youtu.be&fbclid=IwAR18E0Pev5CgLfd8WCxT5Sgal23XilaMFdQ8jQ8onY_byWKc_Ocl79sHnwI)


