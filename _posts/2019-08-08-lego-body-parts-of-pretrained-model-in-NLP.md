---
title: 'Lego body parts of pretrained-models after anatomy of Transfer Learning'
author: yue
layout: post
date: "2019-08-08"
permalink:
categories:
  - Transfer Learning
  - ULMFiT
  - Audio Journal Archive
excerpt: "how to use body parts of pretrained-models after breaking it down and fine-tuning"
---

Prelude:
(1) balance between upsampling folds VS. number of epochs to train for unbalanced dataset in LSTM

- more epochs: trains the nn at a deeper level - generate more minority class prediction even at a very low upsampling scale - but could be false positives

- less epochs but more upsampling folds: trains the nn at a more shallower level - still may be able to quite a few minority class prediction - the false positives VS. true positives are up for an investigation

## Steps of ULMFiT pretrained-models in NLP Transfer Learning:
[Ref: Universal Language Model Fine-Tuning (ULMFiT)
State-of-the-Art in Text Analysis
Authors: Sandra Faltl, Michael Schimpke & Constantin Hackober](https://humboldt-wi.github.io/blog/research/information_systems_1819/group4_ulmfit/)

<img alt="Transfer Learning Work-flow by Sandra Faltl et al." src="https://humboldt-wi.github.io/blog/img/seminar/group4_ULMFiT/Figure_5.png" />

1. Forward pass through the LM in pretrained-model
![Architecture of the Pretrained Model](/images/architecture_pretrained_model.png)

## Q & A

1. What is considered the `word embedding`, the output after embedding layer or the output the entire encoder? How about the **word2vec** & **glove** embeddings? which type are they?

[Audio Journal: Lego body parts of pretrained-models after anatomy of Transfer Learning](https://www.youtube.com/watch?v=IDZzmpSpy-c&feature=youtu.be)

