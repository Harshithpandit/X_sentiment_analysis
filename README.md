Sentiment Analysis using LSTM and TensorFlow
Project Overview

This project performs sentiment analysis on tweets from the Sentiment140 dataset using a Deep Learning approach based on Long Short-Term Memory (LSTM) networks. The model classifies tweets as either positive or negative sentiment.

Dataset
Dataset: Sentiment140
Total Tweets: 1.6 Million
Labels:
0 → Negative Sentiment
1 → Positive Sentiment
Project Pipeline
Data Cleaning
Convert text to lowercase
Remove URLs, mentions, and special characters
Normalize tweet text
Text Preprocessing
Tokenization using Keras Tokenizer
Convert text to integer sequences
Sequence padding for uniform input length
Model Architecture
Embedding Layer
LSTM Layer
Dropout Regularization
Dense Output Layer with Sigmoid Activation
Model Training
Loss Function: Binary Cross Entropy
Optimizer: Adam
Early Stopping to prevent overfitting
GPU accelerated training using Google Colab
Results
Validation Accuracy: ~78%
Successfully classifies positive and negative sentiment in unseen tweets.
Error analysis revealed challenges in handling negation phrases such as:
"not happy"
"not good"
"not bad"
Technologies Used
Python
TensorFlow / Keras
NumPy
Pandas
Scikit-learn
Google Colab
Sample Predictions
Tweet	Prediction
"Virat Kohli played an amazing innings today"	Positive
"I hate waiting in traffic"	Negative
"This movie was fantastic and enjoyable"	Positive
"Worst experience ever"	Negative
Key Learnings
Text preprocessing for NLP
Tokenization and sequence padding
Word embeddings
LSTM architecture
Overfitting detection and mitigation using Dropout and Early Stopping
Model evaluation and error analysis
Future Improvements
Bidirectional LSTM
GRU-based architecture
Pre-trained Word Embeddings (Word2Vec/GloVe)
Transformer-based models such as BERT and DistilBERT
