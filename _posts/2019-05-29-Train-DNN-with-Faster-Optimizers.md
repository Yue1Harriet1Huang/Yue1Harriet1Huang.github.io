---
title: "Train DNN with Fast Optimizers"
author: "yue"
date: '2019-05-29'
excerpt: 
layout: thpost
permalink: /blog/2019/05/faster-optimizers/
categories: Machine Learning Building Blocks
tags:
  - optimizer
---

Note:
Ways to increase DNN training speed:
  - good initialization strategy of connection weights
  - good activation 
  - Batch Normalization
  - transfer learning - pretrained parts
  - faster optimizer

1. Momentum Optimization
---
Motivation: when there is a really smooth elongated valley

Tricks:
- previous gradients affect current gradient
- local gradient serves as the acceleration (a `rate of change` of `rate of change`)
- add friction hyperparameter called the `momentum` between 0 (high) and 1(none)


References
---
Hands-on Machine Learning with Scikit-Learn & Tensorflow
