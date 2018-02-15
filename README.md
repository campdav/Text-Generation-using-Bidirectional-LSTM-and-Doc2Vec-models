# Text-Generation-using-Bidirectional-LSTM-and-Doc2Vec-models
Text Generation using **Bidirectional LSTM** and **Doc2Vec** models

This repository contains jupyter notebooks and data, regarding [this article published on Medium](https://medium.com/@david.campion/text-generation-using-bidirectional-lstm-and-doc2vec-models-1-3-8979eb65cb3a).

The purpose of this article is to discuss about text generation, using machine learning approaches, especially **Recurrent Neural Networks (RNN)** and **Doc2vec**.

Mainly, these approaches are using standard RNN such as LSTM (Long Short-Term Memory), and the are pretty fun to be experimented.

However, generated texts have a taste of unachievement. Generated sentences seem to be quite right, with correct grammar and syntax, as if the neural network was understanding correctly the structure of a sentence. But the whole new text does not have a great sense. And sometimes, has complete nonsense.

This result could come from the approach itself, using only LSTM to generate text, word by word.

In these notebooks, I will try to investigate a new way to generate sentences in a text generator solution.
It does not mean that I will use something completely different from LTSM : I am not. I will use LTSM networks to generate sequences of words. However I will try to go further than a classic LSTM neural network and I will use an additional neural network (LSTM again), to select the best sentences in the text generation.

It will described :
- how to train a neural network to generate sentences (i.e. sequences of words), based on existing novels. I will use a bidirectional LSTM Architecture to perform that.
- how to train a doc2vec model to vectorize sentences,
- how to train a neural network to select the best next sentence for a given paragraph (i.e. a sequence of sentences). I will also use a bidirectional LSTM architecture, in addition with a Doc2Vec model trained on the same target novels.

## Content
This repo contains:
- a **data** folder, with input files
- three **notebooks**:
  - 1 generate sentence: train a bidirectional LSTM to generate sentences, word by word.
  - 2 select sentence: train a Doc2Vec model and a bidirectional LTSM to vectorize sentences
  - 3 generate paragraph: combine all models to generate text
