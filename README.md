# BpHigh@TamilNLP-ACL2022: Effects of Data Augmentation on Indic-Transformer based classifier for Abusive Comments Detection in Tamil
Kernels used for model training using Kaggle Notebooks and other experimental kernels as well as Kernels used for data augmentation purposes.

### `Repo-Visits`
[![Visits Badge](https://badges.pufler.dev/visits/bp-high/BpHigh_at_Dravidian_Lang_Tech_ACL-2022)](https://github.com/bp-high)

### `Background`
* The shared task on Abusive comment detection in Tamil-ACL 2022 is a comment classification problem that can be further described as a multi-class text classification problem in Tamil native script and Tamil-English code-mixed.



* Given a YouTube comment, the systems submitted by the participants should classify its abusive categories.



* The participants were provided with development, training and test dataset in Tamil and Tamil-English. 



* The dataset is tagged using various classes namely, Homophobia, Misandry, Counter-speech, Misogyny, Xenophobia, Transphobic and hope speech.



* The dataset consists of rows that contain the comment text and the label assigned to that comment

### `Contributors`
* Bhavish Pahwa :surfing_man: ([GitHub](https://github.com/bp-high))

### `Methodology`
* We build a classifier using the MURIL Transformer as our embedding layer(all layers frozen) and attach a classifier head by adding subsequent convolution and dense layers. The final output dense layer has softmax activation, which gives us the final predictions.



* We use two data Augmentation approaches to improve our model performance.



* We define an equation to generate a balanced form of the original shared task dataset through our augmentation approaches.



* We take the help of the [NlpAug library](https://github.com/makcedward/nlpaug)
, which provides the methods to perform word-level augmentation using contextual models as well as non-contextual word embeddings like Word2vec, fastText, and Glove.
<p align="center">
<img src="https://github.com/bp-high/BpHigh_at_Dravidian_Lang_Tech_ACL-2022/blob/main/Resources/Classfier_Structure.png" 
     width="500" 
     alt="Classifier Structure"  
     align="center" />
 </p>

