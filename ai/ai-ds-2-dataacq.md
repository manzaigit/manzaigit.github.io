---
layout: post 
title: Data Acqusition 
permalink: /ai/datascience/dataacqusition
---

While we have a lot of data today, there are exceptions:
- Many areas still do not have enough data (e.g. medical) 
- Some data are too dirty (e.g. too many missing values to be of use, sensors didn't capture the data well leading to blurred images)

## Data Sources

It's hard to suggest sources of data without knowing the domain, but here are some general ideas:
- [Google Dataset Search](https://toolbox.google.com/datasetsearch)
- Dataset repositories like [UCI (some quite dated)](https://archive.ics.uci.edu/ml/datasets.php), [Kaggle](https://www.kaggle.com/datasets)
- Open data from the government, usually provided via APIs (e.g. [Data.gov.sg](https://data.gov.sg/))
- Web scraping (ranges from simple to complex)
- IoT, e.g. sensors, using your webcam
- Conducting your own survey via Google Forms / Qualtrics (watch out for data protection / privacy issues!)

## Challenges with real-life data

e.g. Healthcare
- Different + Evolving coding systems for medical terms
- Data governance (e.g. proper de-identification) will eventually be solved but data protection policies and tools take time to refine

## Implementation tips

- It is easier to standardize data than to write code that accomodates to each scenario 
    - If your dataset isn't too big, have a folder of the raw dataset, and have well-named folders for each major step of data cleaning / version
- Folder structure should be kept simple

- Plan data structures properly, think about what you might possibly need
    - Meta-Sim: Learning to Generate Synthetic Datasets
    - Object Annotation with Curve-GCN
    - Data Augmentation
