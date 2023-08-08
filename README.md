# Impact of text sequence size on the performance of deep learning models for sentiment classification.

In this paper, we present our research on how the maximum input size of a plaintext review affects the performance of different deep learning models in sentiment classification. We compared the performance of different maximum text lengths in a deep neural network, a convolutional neural network, and an LSTM. For each model and maximum word length used, we performed the comparison of training the first embedding layer and using a pre-trained by Google known as Word2Vec in order to determine what effect this has on sentiment classification.

We use a public database containing plaintext movie reviews and the rating of each movie. To test with different review sizes, we created datasets with different number of words allowed, as well as a matrix that translates each word found in the data corpus into its respective Word2Vec vector.

Prior to training the models, we performed data cleaning so that the models can use the most relevant information from each review to learn how to classify the sentiment of the reviews. Next, we train the models using each generated dataset both using the Word2Vec vectors and training the embedding layer. Our research reveals that the size of each movie review has an impact on the accuracy of the deep learning models as well as the decision to train or use pre-trained vectors for the embedding layer.

We observed that the LSTM network obtained the best sentiment classification results reaching 88.08% accuracy. Overall, it was beneficial for all tested models to increase the length of words per review. In the case of the DNN and LSTM networks, it was better to train the embedding layer while in the CNN network it was better to use the pre-trained Word2Vec vectors.

This research provides evidence showing how the size of each embedding influences the accuracy of deep learning models. The results are relevant to professionals in the field of artificial intelligence who wish to build sentiment classifiers from plaintext and seek to determine the best way to input their data to an embedding layer in deep learning models.

Dataset used: IMDB Dataset of 50K Movie Reviews. https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews 
