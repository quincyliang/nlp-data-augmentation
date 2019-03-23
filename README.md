# NLP Data Augmentaion

## Overview

- [Task-independent data augmentation for NLP](http://blog.aylien.com/research-directions-at-aylien-in-nlp-and-transfer-learning/)
- [Robust, Unbiased Natural Language Processing](https://drive.google.com/file/d/1JhZKKCJjIDIqZdwRL0GEUcrWxscLS87l/view) [pdf]()



## Methods

- Replacing words with synonyms
  - word embedding,  POS-tag, [link](https://github.com/KonstantinHemker/NLP-data-augmentation)

- Perturbations (letter, word, or sentence level)
  - [noisemix](https://github.com/noisemix/noisemix)

- Language model
  - [Contextual augmentation](https://github.com/pfnet-research/contextual_augmentation)

- Paraphasing
  - Round-trip translation to a different language and back. en > intermediate language > en. [link](https://github.com/PavelOstyakov/toxic/blob/master/tools/extend_dataset.py) 

- [Leverage External Data](https://forums.fast.ai/t/data-augmentation-for-nlp/229/11)
  - Using external data derived from Wikipedia. linking wikipedia articles to arbitrary input text. The idea is that if the input text were on Wikipedia, it would have links to other Wikipedia articles (that are semantically related and provide additional info).
    - break the input text into n-grams
    - check whether each n-gram exists as a wikipedia article to create a set of ‘candidate links’
    - prune the candidate links by computing the similarity of the input text and the abstract of each candidate

-  Machine Translation
  - [low-resource parallel corpuses](https://github.com/fsxfreak/nlp-augment)
  - [back-traslation](https://research.fb.com/publications/understanding-back-translation-at-scale/)

- Conversational Systems
  - [fountain](https://github.com/tzano/fountain)