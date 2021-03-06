# imdb-sentiment-analysis

## Purpose and robustness
The project portrays a simple sentiment analysis program which uses Keras framework and with a 2-layer neural network architecture to predict whether a review is positive or negative. This network is not as robust as an RNN which requires an extra LSTM layer. 

However, this approach could achieve up to 85% accuracy on the test set with very short training time and training data. Certainly by using standard hidden layers with an extra relu layer the network attempts to associate some keywords with the connotation of being 'positive' and some others with 'negative' to determine whether a review is positive or negative. However, it does not take into account the context of the sentence at all which in some cases could manifest in the form of irony and sarcasm. To solve this, an LSTM layer would usually do the trick and more, that is giving better accuracy and taking into account the context of surrounding words, but LSTM layer would require a signficant amount of training time which was too long for my computer to deal with even with a GPU set up. 

Call me lazy but I think this is sufficient to showcase a balance between accuracy and speed for a simple sentiment analysis problem. I might do an LSTM example just to compare the results head-to-head with this network in the future.

## Features

- Train /trained on the imdb dataset from the Keras framework
- Save model locally in json format
- Save weights locally in h5 format
- Visualise training and testing results on matplotlib within the notebook
