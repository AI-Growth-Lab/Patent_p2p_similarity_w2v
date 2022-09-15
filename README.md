# A text-embedding-based approach to measuring patent-to-patent technological similarity

This repository provides adittional documentation and material to the following paper:


* Daniel S. Hain, Roman Jurowetzki, Tobias Buchmann, Patrick Wolf, A text-embedding-based approach to measuring patent-to-patent technological similarity, Technological Forecasting and Social Change, Volume 177, 2022, DOI: [10.1016/j.techfore.2022.121559](https://doi.org/10.1016/j.techfore.2022.121559)
* ArXiv preprint version [here](https://arxiv.org/abs/2003.12303)

* P2P Technological Similarity example: For patent2patent similarity, TF-IDF Weighted W2V was used. For the purpose of testing p2p similarity, we used only 1000 patent abstracts. You can check all steps in the notebook. https://colab.research.google.com/github/AI-Growth-Lab/Patent_p2p_similarity_w2v/blob/main/Patent_W2V_v2_version2_Example.ipynb

### Abstract

This paper describes an efficiently scaleable approach to measuring technological similarity between patents by combining embedding techniques from natural language processing with nearest-neighbor approximation. Using this methodology, we are able to compute similarities between all existing patents, which in turn enables us to represent the whole patent universe as a technological network. We validate both technological signature and similarity in various ways and, using the case of electric vehicle technologies, demonstrate their usefulness in measuring knowledge flows, mapping technological change, and creating patent quality indicators. This paper contributes to the growing literature on text-based indicators for patent analysis. 

### Highlights

* We develop a method to create vector representations of patents based on text data.
* We describe an efficient process to use these vectors to create patent similarity-to-patent measures for large amounts of patents.
* We provide all code and data for reproduction, use, and improvement.
* We evaluate and illustrate the results empirically.
* We illustrate the results of the created measures and metrics at the case of electric vehicle patents.

It contains the following elements:

* Code and demo how to create TFIDF weighted w2v embeddings of patent abstratcs.
* Code and demo how to store the created embeddings in Annoy, and retrieve p2p similarity measures.
* Code and demo how to create aggregated statistics based on p2p similarity measures.
* Full data on created p2p similarity measueres

### Reproducing the model

Before running any code you must install Python3.7+ and requirement libraries:
* Numpy 1.21+
* Gensim 4.1+

The dataset includes 1k patent abstracts as patent_dtatset_sample_1k.csv.

The notebook (Patent_W2V_v2_version2.ipynb) contains all process for preprocessing, training word2vec, computing embeddings, and building trees to tune Annoy (Approximate Nearest Neighbors Oh Yeah).

Queries, comments, and feedback always welcome :)

Also, check out the newest version of SBERT based p2p simialrity measures and automated patent classification.

* [Colab Demo notebooks](https://colab.research.google.com/github/AI-Growth-Lab/Patent_p2p_similarity_w2v/blob/main/Patent_W2V_v2_version2_Example.ipynb)
* [Github](https://github.com/AI-Growth-Lab/Patent-Classification)
* [arXiv](https://arxiv.org/abs/2103.11933)
