---
title: "Data Preprocessing and Python Learning"
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

## Manipulate with Data Structures

Iterate
---

- use asterisk `*` before the iterable data structure such as List, so it iterates through the elements and applies the function
```
l = ["1", "2", "3"]
print(*l) #prints "1", "2", "3" separately element-wise
print(l) #gives the entire list ["1", "2", "3"]
```


[Audio Journal Data Preprocessing - Concatenate, Shuffle, Repeat, Python Tricks](https://www.youtube.com/watch?v=_0MVyKhIqxg&feature=youtu.be)


