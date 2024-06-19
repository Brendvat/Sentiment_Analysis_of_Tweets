This is a Machine Learning and Deep Learning Solution for doing Sentiment Analysis of Tweets.
All the data is mentioned in this repository.
But you have to download this Glove Word Embedding
I am mentioning the steps to do it 
Download the GloVe word embeddings and map each word in the dataset into its pre-trained
GloVe word embedding.
First go to "https://nlp.stanford.edu/projects/glove/" and download the pre-trained embeddings
from 2014 English Wikipedia into the "data" directory. It's a 822MB zip file named glove.6B.zip,
containing 100-dimensional embedding vectors for 400,000 words (or non-word tokens). Un-zip
it. Parse the unzipped file (it's a txt file) to build an index mapping words (as strings) to their
vector representation (as number vectors).
Build an embedding matrix that will be loaded into an Embedding layer later. It must be a matrix
of shape (max_words, embedding_dim), where each entry i contains the embedding_dimdimensional vector for the word of index i in our reference word index (built during
tokenization). Note that the index 0 is not supposed to stand for any word or token -- it's a
placeholder.
