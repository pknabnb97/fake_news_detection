# fake_news_detection_using_word_embedding_and_CNN

This problem was approached as an instance of text classification and only the content of the articles was used as the source
of feature. 
Tensorflow with Keras backend was used for the Tokenization, Pad Sequencing and Model architecture defining tasks.

The model architecture has a word embedding layer that takes input sequences of length the size of the defined vocabulary and embeds them into a vector space of size 16.
Following that, it has convolution layer with units having ReLU activation function and finally a max pooling layer, whose output is finally sent to a sigmoid nonlinearity to predict the label.

The model was then trained for 10 epochs with 99.98% accuracy on the training set and 96% accuracy on the test set.
The loss function was set to ‘binary crossentrophy’ with Adam optimization function and a learning rate of 0.001.
