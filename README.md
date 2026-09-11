# spatula
### or, Slicing Pretrained Audio Transformers to Understand Layerwise Acoustic (features)

Trains probes to predict manner of articulation from internal states of audio encoders.

Code partially adapted from Jon Rawski's LING 165 Lab 1 and Payal Mohapatra's [Speech Disfluency Detection with Contextual Representation and Data Distillation](https://github.com/payalmohapatra/Speech-Disfluency-Detection-with-Contextual-Representation-and-Data-Distillation) Uses [TIMITPhones'](https://github.com/IParraMartin/TIMITPhones/tree/main) map for convenience.

## TODOs:
- verify from a clean install
- remove padding from the whisper emeddings (and voxtral, if it includes padding)

## Usage:
First! Run  `generate_embeddings.ipynb` to generate and save embeddings for both wav2vec, whisper-small, and voxtral mini.

- `probe_training.ipynb` fits probes to predict manner of articulation from the hidden statesaw of the encoders. 


## References:
Cormac English, P., Kelleher, J.D. and Carson-Berndsen, J. ‘Domain-informed probing of wav2vec 2.0 embeddings for phonetic features’, *Proceedings of the 19th SIGMORPHON Workshop on Computational Research in Phonetics, Phonology, and Morphology*, pp. 83–91. doi:10.18653/v1/2022.sigmorphon-1.9. (2022).

Shah, Jui, et al. "What all do audio transformer models hear? probing acoustic representations for language delivery and its structure." *arXiv preprint arXiv:2101.00387* (2021).

Dixit, Satvik, et al. "Explaining deep learning embeddings for speech emotion recognition by predicting interpretable acoustic features." *arXiv preprint arXiv:2409.09511* (2024).

Zhang, Alice, Edison Thomaz, and Lie Lu. "Transformation of audio embeddings into interpretable, concept-based representations." *2025 International Joint Conference on Neural Networks (IJCNN)*. IEEE. (2025).

Fiorio, Luan Vinícius, et al. "Unsupervised Variational Acoustic Clustering." *arXiv preprint arXiv:2503.18579* (2025).

Baevski, Alexei, et al. "wav2vec 2.0: A framework for self-supervised learning of speech representations." *Advances in neural information processing systems 33* (2020): 12449-12460.

Mohapatra, P., Pandey, A., Islam, B., & Zhu, Q. "Speech disfluency detection with contextual representation and data distillation." *In Proceedings of the 1st ACM international workshop on intelligent acoustic systems and applications (pp. 19-24)*. (2022).

Radford, Alec, et al. "Robust speech recognition via large-scale weak supervision." *International conference on machine learning*. PMLR, (2023).

Parra, Iñigo. "TIMITPhones: TIMIT Phoneme Dataset." https://github.com/IParraMartin/TIMITPhones/tree/main. (2025).


Garofolo, John S., et al. TIMIT Acoustic-Phonetic Continuous Speech Corpus LDC93S1. Web Download. Philadelphia: Linguistic Data Consortium, (1993).
