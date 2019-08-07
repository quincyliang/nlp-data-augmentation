# NLP Data Augmentaion

## Paper
- [Unsupervised Data Augmentation](https://128.84.21.199/pdf/1904.12848.pdf) 
- [Unsupervised Question Answering by Cloze Translation](https://arxiv.org/pdf/1906.04980.pdf)
- [Distilling Task-Specific Knowledge from BERT into Simple Neural Networks](https://arxiv.org/pdf/1903.12136.pdf)


## Overview

- [Task-independent data augmentation for NLP](http://blog.aylien.com/research-directions-at-aylien-in-nlp-and-transfer-learning/)
- [Robust, Unbiased Natural Language Processing](https://drive.google.com/file/d/1JhZKKCJjIDIqZdwRL0GEUcrWxscLS87l/view) [pdf](https://github.com/quincyliang/nlp-data-augmentation/blob/master/materials/robust%20training.pdf)

## Methods

- General 
  - random insertion, deletion, word, sentence shuffling
- [Replacing words with synonyms](https://github.com/KonstantinHemker/NLP-data-augmentation)
- Replace the words from dicitionary of the same label
  - [NER](https://zhuanlan.zhihu.com/p/43061858)
- Perturbations (letter, word, or sentence level)
  - [noisemix](https://github.com/noisemix/noisemix)
- Language model
  - [Contextual augmentation](https://github.com/pfnet-research/contextual_augmentation)
- Back translation
  - [Machine traslation](https://research.fb.com/publications/understanding-back-translation-at-scale/)
- Round-trip translation
  - [Paraphasing](https://github.com/PavelOstyakov/toxic/blob/master/tools/extend_dataset.py)
  - [Low-resource parallel corpuses](https://github.com/fsxfreak/nlp-augment)
  - [中文文本纠错任务](https://liweinlp.com/?p=5000)
- [Leverage External Data](https://forums.fast.ai/t/data-augmentation-for-nlp/229/11)
  - Using external data derived from Wikipedia. linking wikipedia articles to arbitrary input text. The idea is that if the input text were on Wikipedia, it would have links to other Wikipedia articles (that are semantically related and provide additional info).
    - break the input text into n-grams
    - check whether each n-gram exists as a wikipedia article to create a set of ‘candidate links’
    - prune the candidate links by computing the similarity of the input text and the abstract of each candidate
- Conversational Systems
  - [fountain](https://github.com/tzano/fountain)
- Reading Comprehension 
  - [Entity replacement and permutation](https://papers.nips.cc/paper/5945-teaching-machines-to-read-and-comprehend.pdf)
  - [Generate strong negatives based on POS tags](https://github.com/quincyliang/nlp-data-augmentation/blob/master/materials/jdevlin.pdf)


## Library
- [nlaug](https://github.com/makcedward/nlpaug)

  
