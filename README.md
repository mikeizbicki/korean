# Notes on Korean language NLP

1. Linguistics Books:
    
    *A History of the Korean Language* by Ki-Moon Lee and S Robert Ramsey

    *The Korean Language* by Ho-Min Sohn

    *The Korean Language: Structure use and context* by Jae-Jung Song

## Word Vectors

1. https://aclanthology.org/D17-1075/

    Decompose words into their jamo representation (versus their character/syllable representation) before passing them to a BiLSTM.  Application is dependency parsing.  Code available.


1. https://aclanthology.org/P18-1226/

    Extends fasttext from a syllable based method on korean to a jamo based method.
    Similar to the Stratos paper above, but focuses on word embedding evaluation rather than the downstream task.

    Code at: https://github.com/SungjoonPark/KoreanWordVectors

1. https://aclanthology.org/D19-1358/

    Introduce the Hanja-level Subword Information Skip-Gram (SISG) model for Korean word vectors, which uses both Hanja (Chinese characters) and hangul to create embeddings.
    They specifically reference the limitations of fasttext for hangul.

    Intro has a good overview of Chinese/Korean linguistic history with refs.    

    Code at https://github.com/kaniblu/hanja-sisg

## 

1. https://aclanthology.org/2020.lrec-1.429/

    Argues that Korean (and CJK more generally) is particularly challenging for multilingual models (like multilingual-BERT) due to the initial tokenization step.
    Introduces a new way of tokenizing Korean to improve these models,
    but does not seem to actually train a new BERT model.

1. Korean BERT models:
    1. https://github.com/sktbrain/kobert
    1. https://github.com/yeontaek/bert-korean-model

## Sentiment

1. https://aclanthology.org/2020.lrec-1.199/

   Introduce Korean Movie Review Emotion (KMRE) Dataset and a Korean-specific method for emotion prediction.

1. https://www.sciencedirect.com/science/article/abs/pii/S0306457318305612
