**The goal of this project was to predict the sentiment of a given tweet.**

Provided a dataset that contained tweets labeled as positive, negative, or nuetral, 
I achieved this objective by building a NLP sequencing model with TensorFlow.

How I approached this problem.
1) Obtain the data
2) Explore the data for greater understanding.
3) Preprocess and sequence the text and one-hot encode the labels.
4) Build model with an embedding, Bidirectional GRUs, and a final Dense output layer.
5) Plot model training accuracy vs validation accuracy to understand performance and tune hyperparameters appropriately.  In this case, the model was overfitting (which is common for NLP because the chances that the training data is not fully representative of the testing data is high, since there are many words, abbrevations, and slang in written language). To combat this I increased recurrent_dropout and dropout in my Bidirectional GRU layers.  I also experimented with the vocabulary size and embedding dimensions, among others.  I also chose to train for very few epochs.
6) Create visualizations of the trained model for greater understanding.
7) Build a method to make predictions!
