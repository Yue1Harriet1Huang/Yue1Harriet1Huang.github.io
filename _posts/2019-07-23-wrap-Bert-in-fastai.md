---
title: "Wrap BERT in fastai"
author: "yue"
date: '2019-07-23'
excerpt: "My experiences in learning wrapping BERT in fastai"
layout: post
permalink: /blog/2019/07/wrap-Bert-in-fastai/
categories:
  - Transfer Learning 
  - BERT
  - fastai
  - Audio Journal Archive
---

## The components to run fastai ULMFiT process

1. fastai Tokenizer 
```
fastai.text.transform.BaseTokenizer
fastai.text.transform.Tokenizer wraps not inherits a fastai SpacyTokenizer which inherits a BaseTokenizer
```
**wrap BertTokenizer into a fastai Tokenizer**

Design decision:

(1) a new tokenizer class called `FastaiBaseBertTokenizer` that can convert/type cast a `BertTokenizer` into a fastai `BaseTokenizer`
(2) since a fastai `Tokenizer` class can already takes in/type cast a BaseTokenizer object, I am going to let the new defined FastaiBaseBertTokenizer object be able to return a fastai Tokenizer object built on top of a converted BaseTokenizer object from BertTokenizer and I am going to define this as a static method of the newly defined class FastaiBaseBertTokenizer, or you can also just use Tokenizer to typecast directly.

```
from pytorch-pretrained_bert import BertTokenizer

class FastaiBaseBertTokenizer(BaseTokenizer):
    def __init__(tok: BertTokenizer, **kwargs):
    
    @staticmethod
    def get_fastai_tokenizer(tok: SpacyTokenizer):
        return(Tokenizer(tok))
    

```
2. vocabulary from the tokenizer
3. fastai TextDataBunch
4. fastai learner 





[Audio Journal Data Preprocessing - Concatenate, Shuffle, Repeat, Python Tricks](https://www.youtube.com/watch?v=_0MVyKhIqxg&feature=youtu.be)


