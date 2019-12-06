---
layout: post 
title: Neural Networks
permalink: /ai/neuralnetworks
---

## Hyperparameters

1. Learning Rate
    Adaptive learning rate / Decay
2. Number of layers
3. Number of nodes in each layer
4. Weight decay
5. Regularization
6. Dropout

Reproducibility is important, but might not be possible in some situations (e.g. if you're using [Keras and a GPU setup](https://github.com/keras-team/keras/issues/12800)). There are [upcoming solutions](https://github.com/NVIDIA/tensorflow-determinism) though, and here's how to achieve it with a [CPU-only setup](https://keras.io/getting-started/faq/#how-can-i-obtain-reproducible-results-using-keras-during-development).

