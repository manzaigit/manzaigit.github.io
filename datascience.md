---
layout: page
title: Data Science
permalink: /datascience/
order: 2
---

There are already a lot of data science articles in the web, but this list of articles is different as it gives a holistic (both business-centric and technical) view of Data Science. I guess we can call it full-stack data science ;)

- Math
- Business Problem and Requirements Analysis
- A software engineering approach to data
- Data pipeline
- [AI](/datascience/ai)

Always start small and iterate. 
Write to CSV files, save your outputs
Write test cases 

After all, machine learning only plays a small part 

AI Transformation Playbook How to lead your company into the AI era - Landing AI

## Understanding the business

10 Reads for Data Scientists Getting Started with Business Models — Conor Dewey

## Getting Data
- Meta-Sim: Learning to Generate Synthetic Datasets
- Object Annotation with Curve-GCN
- Data Augmentation


## Challenges with real-life data
e.g. Healthcare
- Different + Evolving coding systems for medical terms
- Current system is based on 
- Data governance (e.g. proper de-identification) will eventually be solved but data protection policies and tools take time to refine

Implementing data-driven change
At the start, we mentioned that insights generated from data have to be actionable. What's even more important is getting the organisation to execute it.

However, creating organisational change is not trivial. 

Incentive -> Monitoring -> Re-inforce 

References
- https://www.bain.com/insights/with-advanced-analytics-its-people-not-data-that-stand-in-the-way-of-change


## Visualisation

## Modelling

- Universal Approximation Theorem (George Cybenko in 1988 showed that *any* function can be approximated to arbitrary accuracy by a NN with 3 layers (2 hidden, 1 output), works in the condition that the number of hidden units is unbounded)

[1812.10156] Deep neural networks are biased towards simple functions

Handling class imbalance
* Focal loss @ retinanet
* SkewFit by Pong et al?
* https://arxiv.org/abs/1805.03901
* https://imbalanced-learn.readthedocs.io/en/stable/


Debugging / Improving
- Use deconvolutional nets to analyse CNN and see what can be improved (e.g. increase filter size, reduce stride)

## Reporting

D3.js is interesting but a little too low-level (it's your best bet if you want something highly customizable, if you're just building normal visualisations there will be alternatives like ___)

## Maintaining

- Online learning
- Failing Loudly: An Empirical Study of Methods for Detecting Dataset Shift

Last updated: 25 July 2019