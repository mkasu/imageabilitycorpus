# Multi-modal Imageability Corpus

This is a (work in progress) corpus on multi-modal imageability norms. 

## (Preliminary) Dataset

Currently 118 words (testing data from [2]).

_We are working on increasing this corpus in future._

## Estimated values

- Visual features from [1]: 
	- Low-level features (SURF, GIST, Color histograms)
	- High-level features (Object detection, Categories)
- Language features from [2]:
	- Pretrained Word embedding (FastText)
- Phonetic features from [2]:
	- Bag-of-Words model with using IPA values instead of words
	- Vectorized word pronunciation model using LSTM

## Implementations

[1] (using only visual features) is available at: https://github.com/mkasu/imageabilityestimation

[2] is planned to be made available in future.

## Publications

[1] Estimating the imageability of words by mining visual characteristics from crawled image data. Marc A. Kastner, Ichiro Ide, Frank Nack, Yasutomo Kawanishi, Takatsugu Hirayama, Daisuke Deguchi, Hiroshi Murase. Multimed Tools Appl, 79(25), 18167-18199, February 2020. https://doi.org/10.1007/s11042-019-08571-4.

[2] Imageability estimation using visual and language features. Chihaya Matsuhira, Marc A. Kastner, Ichiro Ide, Yasutomo Kawanishi, Takatsugu Hirayama, Keisuke Doman, Daisuke Deguchi, Hiroshi Murase. ACM International Conference on Multimedia Retrieval (ICMR) 2020, June 2020. https://doi.org/10.1145/3372278.3390731
