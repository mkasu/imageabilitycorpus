# Multi-modal Imageability Corpus

This is a corpus on multi-modal imageability norms. This dataset is part of the paper [3].

## Imageability 

Imageability is "the ease with which a word gives rise to a sensory mental image" (Paivio, Yuille & Madigan. Concreteness, imagery, and meaningfulness values for 925 nouns. 1968) There are psycholinguistic corpora which are created by hands through crowd-sourcing. 

We believe imageability as an extra source of knowledge can be very promising for multi-modal research as it connects to both visual and language stimuli. For example, it gives hints at whether something is visually ambiguous or not, perceived as abstract or concrete, and so on.

In our research, we proposed to estimate imageability norms for words from large image and text corpora using data-mining techniques.

## Corpus

Currently __2430 English words__ with estimated values for visual, language, and phonetic features. The _ety_ field shows an estimated origin etymology (created using [Etymological Wordnet](http://etym.org)) and the _pos_ field shows an estimated part-of-speech (created using WordNet and NLTK).

`corpus_icmr2020.csv`: Testing data used in [2]: 118 English words.

`corpus_mipr2021.csv`: Dataset created for [3]: 2430 English words.

_We are working on increasing this corpus in future._

## Estimated values

The data contains estimated values for three different modalities:

- __Visual__ features data-mined from 5000 images per word (based on a modified model of [1]+[2]): 
	- Low-level features (SURF, GIST, Color histograms)
	- High-level features (Object detection, Categories)
- __Language__ features data-mined from large-scale text corpus (used [2]):
	- Pre-trained word embedding (FastText)
- __Phonetic__ features data-mined from word-pronunciation data (based on a modified model of [2]):
	- Bag-of-Words-like model using IPA values of words pronunciation
	- LSTM-based model to vectorize word pronunciation

More details of this are discussed in [3].

Each value is given in an interval of [100, 700], corresponding to the Lickert scales used in Psycholinguistic dictionaries (the most common being [1, 5] and [1, 7]).

## Dataset visualizations

Some dataset visualizations were created as part of [3]. The demos showcased in the paper are available at https://www.marc-kastner.com/mipr2021viz/index.html.

## Implementations

[1] (using only visual features) is available at: https://github.com/mkasu/imageabilityestimation

[2] (extending [1] with language and phonetic features) is planned to be made available in future.

## Publications

[1] Estimating the imageability of words by mining visual characteristics from crawled image data. Marc A. Kastner, Ichiro Ide, Frank Nack, Yasutomo Kawanishi, Takatsugu Hirayama, Daisuke Deguchi, Hiroshi Murase. Multimed Tools Appl, 79(25), 18167-18199, February 2020. https://doi.org/10.1007/s11042-019-08571-4.

[2] Imageability estimation using visual and language features. Chihaya Matsuhira, Marc A. Kastner, Ichiro Ide, Yasutomo Kawanishi, Takatsugu Hirayama, Keisuke Doman, Daisuke Deguchi, Hiroshi Murase. ACM International Conference on Multimedia Retrieval (ICMR) 2020, June 2020. https://doi.org/10.1145/3372278.3390731.

[3]	A multi-modal dataset for analyzing the imageability of concepts across modalities. Marc A. Kastner, Chihaya Matsuhira, Ichiro Ide, Shin'ichi Satoh. IEEE International Conference on Multimedia Information Processing and Retrieval (MIPR2021), To be published in September 2021.

