# Multi-modal Imageability Corpus

This is a (work in progress) corpus on multi-modal imageability norms. 

## Preliminary corpus

Currently 118 English words (testing data used in [2]).

_We are working on increasing this corpus in future._

## Estimated values

- Visual features data-mined from 5000 images per word ([1]+[2]): 
	- Low-level features (SURF, GIST, Color histograms)
	- High-level features (Object detection, Categories)
- Language features data-mined from large-scale text corpus ([2]):
	- Pre-trained word embedding (FastText)
- Phonetic features data-mined from word-pronunciation data ([2]):
	- Bag-of-Words-like model using IPA values of words pronunciation
	- LSTM-based model to vectorize word pronunciation

## Implementations

[1] (using only visual features) is available at: https://github.com/mkasu/imageabilityestimation

[2] (extending [1] with textual and phonetic features) is planned to be made available in future.

## Publications

[1] Estimating the imageability of words by mining visual characteristics from crawled image data. Marc A. Kastner, Ichiro Ide, Frank Nack, Yasutomo Kawanishi, Takatsugu Hirayama, Daisuke Deguchi, Hiroshi Murase. Multimed Tools Appl, 79(25), 18167-18199, February 2020. https://doi.org/10.1007/s11042-019-08571-4.

[2] Imageability estimation using visual and language features. Chihaya Matsuhira, Marc A. Kastner, Ichiro Ide, Yasutomo Kawanishi, Takatsugu Hirayama, Keisuke Doman, Daisuke Deguchi, Hiroshi Murase. ACM International Conference on Multimedia Retrieval (ICMR) 2020, June 2020. https://doi.org/10.1145/3372278.3390731
