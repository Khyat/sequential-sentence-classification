# Sequential Sentence Classification [SkimLit]

In this particular repository, I've replicated the deep learning model behind the 2017 paper [PubMed 200k RCT: a Dataset for Sequential Sentence Classification in Medical Abstracts](https://arxiv.org/abs/1710.06071)

When it was released, the research paper presented a new dataset called PubMed 200k RCT which consists of ~200,000 labelled Randomized Controlled Trial (RCT) abstracts.

The goal of the dataset was to explore the ability for NLP models to classify sentences which appear in sequential order. In other words, given the abstract of a RCT, what role does each sentence serve in the abstract?

## Problem Statement

The number of RCT papers released is continuing to increase, those without structured abstracts can be hard to read and in turn slow down researchers moving through the literature.

## What this notebook covers?

1. You can download the text dataset from here [PubMed RCT200k from GitHub](https://github.com/Franck-Dernoncourt/pubmed-rct)
2. Writing a preprocessing function to prepare our data for modelling
3. Setting up a series of modelling experiments
     - Developing a baseline model (TF-IDF Classifier)
       - Deep learning models with different combinations of: token embeddings, character embeddings, pretrained embeddings, positional embeddings
4. Building our first multimodal model (taking multiple types of data inputs)
     - Replicating the model architecture from [Neural Networks for Joint Sentence Classification in Medical Paper Abstracts](https://arxiv.org/pdf/1612.05251.pdf)
  
