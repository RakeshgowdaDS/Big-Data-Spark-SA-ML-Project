# Big-Data-Spark-SA-ML-Project

Tweet Sentimental Analysis using Spark and ML

This project aims to understand and analyze machine learning tasks on large data streams. We have chosen the “Sentiment140” dataset. 

The CSV dataset is encoded into JSON and then it is streamed via TCPsocket. Then the stream is received using the readstream() function with 
the source as a socket.

After receiving a batch of data, it is Pre-Processed.

After Pre-Processing we are building models for clustering and classification -
  1.Classification models – SGD Classifier, PassiveAggresive Classifier
  2.Clustering Model – Mini-batch K-Means 

The aforementioned models are trained on each batch of data.

After training the models on the whole dataset we use them to predict the test batches.

F1 score, precision, recall, and accuracy are calculated. 

