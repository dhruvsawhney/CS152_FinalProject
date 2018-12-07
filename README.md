# CS152_FinalProject (Neural Networks)

Project: Sentiment Analysis on IMDB movie reviews using Recurrent Neural Network
        Prediction: 1/0 for a positive/negative movie review sentiment
        Data Source: Kaggle IMDB movie review (https://www.kaggle.com/c/sentiment-analysis-on-movie-reviews/data)

2 models have been implemented:

1. Sentiment Analysis using word embedding (RNN_with_word_embedding.ipynb)

  An RNN (architecture details in notebook) using the Keras deep-learning framework. Furthermore, I use a word-embedding layer
  (GloVe embedding) that takes the raw text and feeds dense vector embeddings as input to the RNN.
  
2. Sentiment Analsis using Transfer Learning (TransferLearning.ipynb)
  
  This approach is modelled after the paper (https://arxiv.org/abs/1801.06146) and implementation (https://github.com/fastai/fastai/blob/master/courses/dl1/lesson4-imdb.ipynb).
  
  The goal is to recreate this paper to perform transfer learning for sentiment classification, by first creating a language model based on a corpus of text.
  Finally, this model is tuned to perform sentiment classification. Techniques used to train the LM for sentiment analysis can be found in the paper and notebook.
  
  The corpus used for training the language model is another IMDB dataset. Then, transfer learning is performed using the Data Source (cited above).
