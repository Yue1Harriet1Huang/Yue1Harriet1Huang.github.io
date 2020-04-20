---
title: "How to creat a pypi package that can be downloaded through pip on your own github repo"
author: yue
layout: post
permalink:
categories:
  - Audio Journal Archive
excerpt: ""
---

1. one more folder with the same name as the package name 
2. `setup.py` file outside of the new package folder and inside the original folder
3. `__init__.py` file inside the new folder 
4. how to add to requirements.txt to `pip install` your new repo, `pip upgrade` the packages in requirements.txt
5. public versus private repo: https versus git ssh


{% include image.html url="/images/donald-trump.jpg" caption="The Trump phenomenon has exposed an undercurrent in American values that World Values Survey researchers have known well." width=450 align="bottom" %}
