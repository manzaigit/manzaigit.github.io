---
layout: post 
title: Modelling
permalink: /ai/datascience/modelling
---

tl;dr:


Although modelling only plays a small part in a data science project (some say that it's only a few lines of code, but that's because all the complexity is wrapped within a function), it's one of the richest and most complicated areas of data science.

Your goal should not be to plug the latest model to your use case.

After all, machine learning only plays a small part 



Statistical software / ML models often have default parameters set
e.g. sklearn, LR has L2 regularisation (@ C=1)

Feature Scaling: Many ML algorithms use Euclidian distance -> need feature scaling if order of magnitude varies significantly 
- z-score, mean normalisation [-1,1], min-max [0,1] 


- Universal Approximation Theorem (George Cybenko in 1988 showed that *any* function can be approximated to arbitrary accuracy by a NN with 3 layers (2 hidden, 1 output), works in the condition that the number of hidden units is unbounded)

[1812.10156] Deep neural networks are biased towards simple functions

Handling class imbalance
* Focal loss @ retinanet
* SkewFit by Pong et al?
* https://arxiv.org/abs/1805.03901
* https://imbalanced-learn.readthedocs.io/en/stable/

Overfitting


Debugging / Improving
- Use deconvolutional nets to analyse CNN and see what can be improved (e.g. increase filter size, reduce stride)
