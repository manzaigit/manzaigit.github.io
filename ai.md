---
layout: page
title: AI
permalink: /AI/
order: 3
---

*Last updated: 17 May 2020*

tl;dr
- What AI is and the tribes of AI 
- Current progress and possible future directions
- Important considerations for AI Deployment

**Definition** 

Artificial Intelligence, Machine Learning and Deep Learning were part of the buzzwords used in the 2010s, and a consensus that AI ⊃ ML ⊃ DL was arrived at. There is less consensus on the definition of intelligence, but here's a working definition paraphrased from [Lexico](https://www.lexico.com/en/definition/intelligence): ability to receive, process and apply information. This entails a sensitive sensory system and adaptive motor mechanism. It's no trivial matter to come up with high-resolution sensors and 'actuators' with fine motor control, but [understanding](https://medium.com/@tdietterich/what-does-it-mean-for-a-machine-to-understand-555485f3ad40) is particularly hard because it implies an ability to break down ideas and concepts into fundamental parts, explain the links between them, identify adjacencies and generate future possibilities / implications from these information. The goal of AI [^1] is to create such forms of understanding in machines but we are still very far from the end goal. 

**Current Progress**

In brief, we have powerful models that can learn patterns from large datasets, but they offer limited interpretability and are harder to train with limited data. We've had interpretable models, but they are often outperformed and usually requires more effort to convert complex datasets (images, video) into features that can be used as inputs. We still don't have models that can perform on par with humans in terms of:

1. Size of datasets (humans can generalize from fewer samples than our models)
2. Data modalities (our brains take in auditory, visual, olfactory information simultaneously)
3. Model interpretability (we can explain how and why we arrive at certain conclusions)

**Future Directions**

AI has outperformed humans in specific tasks, but what does it take to develop models that can generalize better? Using the 3 aspects mentioned above in the context of 'traditional' ML and DL models[^2]:

1. *Size of datasets*: ML models can't capture complex patterns easily and lose out in big datasets, while DL models might be too sensitive to noise especially in small datasets. Unlike humans, they do not have common sense / a causation prior to avoid illogical patterns - just because a feature has high values for class A and low values for class B does not mean that it is important, or that it is a causal factor leading to the class difference.

2. *Data modalities*: ML models require some form of feature extraction to convert complex datasets into learnable formats (e.g. windowing time series data, SIFT vs CNN for images), losing critical information in the process. On the other hand, the breadth of DL models (CNN, RNN, GNN) makes it possible for a larger variety of data to be modeled directly. Unlike humans, we aren't so good at merging multiple modalities yet and I think the eventual shift to multimodal dataset and methods in the next decade (we've had much progress but they have largely been on unimodal data) will lead to a lot of significant performance improvements if we curate the datasets well. 

3. *Interpretability*: ML models like decision trees and CART make their decision making process very clear, but DL models have limited interpretability for now (e.g. identifying important features based on weights or perturbations to the inputs). Though complex, I don't see DL models are black boxes - the model starts off from an initial state (most always with wrong predictions) and makes adjustments to model parameters based on gradient computations that stemmed from the minimization of a loss function. That implies that the series of changes made on model parameters should be attributable to specific groups of incorrect predictions that contribute the most to the loss function, and we are theoretically able to assign credit to these data samples and features. The specific samples and features that plays the greatest role in the model training process could vary over iterations, creating much complexity but that does not make it a black box - it's just that no one has reached this level of understanding yet.

**Symbolists, Connectionists, Bayesians, Evolutionaries, Analogizers**

More generally (beyond ML/DL), there have been many proposed systems for creating understanding in machines (grouped into [5 tribes](https://kevinbinz.com/2017/08/13/ml-five-tribes/) in Pedro Domingos’ book 'The Master Algorithm'). The most intuitive way is to come up with rules and knowledge bases with ontologies, but they do not always generalize well and we still do not have many algorithms that create them dynamically at an acceptable performance level. Alternatively, we could do without explicit task-based instructions and build models for machines to learn from data, with the advantage of learning more adaptable 'rules' but with the disadvantage of losing interpretability especially when the models used increase in complexity. Despite the differences in approaches, one key limitation shared by all of them is the hypothesised presence of a **semantic gap** between humans and computers. What we see as words, colors and pictures can only be represented as numbers in computers. I see this as a key limitation (that we often forget) and a differentiator between humans and AI, but it hasn't stopped modern AI from being useful. 

**Deployment**

Given the rapid pace of AI research, all kinds of model architectures are proposed everyday but AI is much more than just creating new models. As Andrew Ng mentioned in The Batch, getting it to work requires (i) technical advancements in getting models to work on [small datasets](https://info.deeplearning.ai/the-batch-self-driving-cars-that-cant-see-pedestrians-evolutionary-algorithms-fish-recognition-fighting-fraud-), addressing biases, improving explainability / interpretability and ensuring [robustness](https://info.deeplearning.ai/the-batch-deepmind-masters-starcraft-2-ai-attacks-on-amazon-a-career-in-robot-management-banks-embrace-bots-1), (ii) [business considerations](https://blog.deeplearning.ai/blog/the-batch-google-achieves-quantum-supremacy-amazon-aims-to-sway-lawmakers-ai-predicts-basketball-plays-face-detector-preserves-privacy-problems-beyond-bounding-box) such as starting small before scaling up (and proper project management, as rigourous and mature as traditional software engineering), clear communication of what AI can and cannot offer[^3] to stakeholders, whether the AI solution addresses the problems faced by end-users (and they are able to integrate it into their workflow) and having regular audits / tests of model performance. I think the most effective teams are multidisciplinary, made up of domain experts with extensive experience and a basic understanding of AI concepts + AI-trained developers who have sufficient experience in the domain. Such a mix ensures that they are at least able to generate feasible ideas, set realistic goals and communicate well. Curating a knowledge base of AI concepts for domain experts (and a useful reference for AI developers) is quite a huge task and I've split it into 3 parts with a healthy mix of theory, practical and business considerations.

* Math and Statistics (just enough to understand the other topics well)
* [Data Analytics and Machine Learning (theory and practice in businesses)](/ai/datascience)
* Knowledge Representation and Deep Learning Applications

Fundamentally, we need to keep in mind that the high accuracies reported in papers are almost always on static datasets but the world is [dynamic](https://info.deeplearning.ai/the-batch-deepmind-masters-starcraft-2-ai-attacks-on-amazon-a-career-in-robot-management-banks-embrace-bots-1) and we need to know when and where we should not rely on AI (e.g. when historical data does not help to explain the present; fundamental shifts).

<!-- Physics and AI -->

🤖

Footnotes:

[^1]: More formally, AI is defined by Patrick Winston (in the MIT 6.034 course) to be: "Algorithms enabled by constraints which are exposed by representations that support the building of models targeted at perception, thinking and action". To have a model, you need representation -> getting the right representation will expose constraints of the problem (e.g. algebra, algebraic notation exposes constraints that make it possible to figure out the problem/relations).

[^2]: Many more important aspects not covered includes multi-label and multi-task problems, semi-supervised learning, the role of [self-supervised learning](https://www.facebook.com/yann.lecun/posts/10156437493897143) and teaching AI how to plan and reason. Multi-label: each object inherently contains more information than what we are currently tagging - we have only given AI a limited view of the world. 

[^3]: Even if the models are well trained, the data you get in deployment settings are quite likely to be [different from what was used for training](https://www.technologyreview.com/2020/04/27/1000658/google-medical-ai-accurate-lab-real-life-clinic-covid-diabetes-retina-disease/). People do what is convenient for them and that could affect the quality of data. 