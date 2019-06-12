# DL-for-NLP
DL for NLP Word2Vec embedding
Description: Experiments with DL for NLP.
You are expected to use the Python language and the Keras library unless otherwise noted. You will prepare a report including your code and results (in a Jupyter Notebook). The report format is shown at the end of this document.
You will use a version of Wikipedia in Turkish as corpus for this homework. The data can be accessed at https://gtu-my.sharepoint.com/:u:/g/personal/yakup_genc_gtu_edu_tr/EaX_gOTBvn5In0LMYXr6oUcBU_mv3U3Ka7WbCKUS011Prg?e=K1dXJr
Part 1: Prepare your data
Use Word2Vec embedding as discussed in class or whatever you see fit for this problem. Some sort of word embedding will be needed.
Part 2: NextWordPrediction
Train a network that can predict the next word given a set of words of a sentence. Use the trwiki text for obtaining the data.
Training data is formed from the corpus by jut using a set of words followed by the next word. For example, if you are given the following as the corpus:

![Capture](https://user-images.githubusercontent.com/32982938/59377991-03b1c380-8d5c-11e9-89ea-ee6cae1bd60b.PNG)



Part 2.1: NextWordPrediction using only last 4 previouswords using CNN
The first algorithm for word prediction will use always four input words followed by a fifth word to be predicted. The above examples become:
Training data:
![Captfffure](https://user-images.githubusercontent.com/32982938/59378179-673bf100-8d5c-11e9-8d55-acac275a306d.PNG)

Use perplexity measure to measure the performance of your algorithm.
Part 2.2: NextWordPrediction using arbitraray many previous words using LSTM
This time assume that you can use the original data sequence above. For this, you musht use an LSTM-like algorithm as the data may have varying number of words as input.
Use perplexity measure to measure the performance of your algorithm.
Part 3: NextWordPredictionGivenPartialWord
Training data is formed from the corpus by just using a set of words followed by the next word:
Makine  ö
Makine ö  ğrenimi
Makine öğ  renimi
Makine öğr  enimi
…
Makine öğrenimi  ‘ ‘
Makine öğrenimi  b
Makine öğrenimi b  i
Testing…
B  u
Bu  n
Bun  u
Bunu  n
…
Use perplexity measure to measure the performance of your algorithm.
