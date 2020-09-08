# Multi-modal Imageability Corpus

This is a (work in progress) corpus on multi-modal imageability norms. 

## Imageability 

Imageability is "the ease with which a word gives rise to a sensory mental image" (Paivio, Yuille & Madigan. Concreteness, imagery, and meaningfulness values for 925 nouns. 1968)

There are psycholinguistic corpora which are created by hands through crowd-sourcing. We believe imageability as an extra source of knowledge can be used for multi-modal research as it connects to both visual and language stimuli. 

In our research, we proposed to estimate imageability from large image and text corpora using data-mining techniques.

## Preliminary corpus

Currently 118 English words (testing data used in [2]).

_We are working on increasing this corpus in future._

## Estimated values

The data contains estimated values for three different modalities:

- Visual features data-mined from 5000 images per word ([1]+[2]): 
	- Low-level features (SURF, GIST, Color histograms)
	- High-level features (Object detection, Categories)
- Language features data-mined from large-scale text corpus ([2]):
	- Pre-trained word embedding (FastText)
- Phonetic features data-mined from word-pronunciation data ([2]):
	- Bag-of-Words-like model using IPA values of words pronunciation
	- LSTM-based model to vectorize word pronunciation

A combined value is also provided.

Each value is normalized between [0, 100], but the values correspond to the Lickert scales used in Psycholinguistic dictionaries (the most common being [1, 5] and [1, 7]).

## Implementations

[1] (using only visual features) is available at: https://github.com/mkasu/imageabilityestimation

[2] (extending [1] with textual and phonetic features) is planned to be made available in future.

## Publications

[1] Estimating the imageability of words by mining visual characteristics from crawled image data. Marc A. Kastner, Ichiro Ide, Frank Nack, Yasutomo Kawanishi, Takatsugu Hirayama, Daisuke Deguchi, Hiroshi Murase. Multimed Tools Appl, 79(25), 18167-18199, February 2020. https://doi.org/10.1007/s11042-019-08571-4.

[2] Imageability estimation using visual and language features. Chihaya Matsuhira, Marc A. Kastner, Ichiro Ide, Yasutomo Kawanishi, Takatsugu Hirayama, Keisuke Doman, Daisuke Deguchi, Hiroshi Murase. ACM International Conference on Multimedia Retrieval (ICMR) 2020, June 2020. https://doi.org/10.1145/3372278.3390731
