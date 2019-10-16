---
title: Info Geometric
date: 2018-09-11
image: images/blog/fig_1_process.png
author: Admin
---

# Zhihu Sentiment Classification
## Introduction

With the development of the Internet, a large number of users on the Internet have writen a lot of text,which contain the people’s sentiment. However, due to the huge amount of text, it is impossible to deal with the amount of text on the Internet only by relying on manual means. So we need a Intelligent algorithm to classify the sentiment of text automatically.

This project aims to develop a sentiment classification system to classify the emotional polarity for Zhihu text.

## Problem
We got some labeled datasets from Zhihu company, The problem are as follows：
  
1. The datasets are very small and the data distribution is uneven
1. Emotional semantics are not obvious，and emotional expression is implicit

## Methodology
1. Based on emotion dictionary and machine learning
        Due to the serious over-fitting phenomenon of neural network, we tried to use the related methods of supervised learning based on the emotional dictionary to ensure that all texts are labeled to a specific emotional polarity. The specific process is shown in the figure1:
        ![](../../../images/blog/fig_1_process.png)
1. Fine-tuning method based on BERT pretrain model
        Due to the lack of training corpus, we used the pre-train model with the best text classification model BERT to infer the emotional polarity, the structure is shown as folleow:
        ![](../../../images/blog/bert.png)
1. Fastext
        FastText is a text classifier opened by Facebook AI Research in 2016, which has good performance in text classification task. Its structure is shown in the following figure:
        ![](../../../images/blog/fastext.png)