Spell Checker
The objective of this project is to build a model that can take a word with spelling mistakes as
input, and output the same word with the mistakes corrected. For e.g. wrk would return work.
The data that we will use for this project will be Google’s 1 billion word corpus.
We will be using pre-trained model word2vec and train it on the dataset: Google’s 1 billion word
corpus and test it on test set and as word2vec produces each unique word in the corpus being
assigned a corresponding vector in the space. Word vectors are positioned in the vector space
such that words that share common contexts in the corpus are located in close proximity to one
another in the space so this way if we would input a word with wrong spelling then it will output
the correct spelling which is the closest match to the input.
There are two architectures for implementing Word2Vec:
 CBOW (Continuous Bag-Of-Words) and
 Skip-gram
In this implementation, we'll be using the skip-gram architecture because it performs better than
CBOW.
The process of implementation is as follows:
 Loading the Data
 Preparing the Data
 Building the Model
 Training the Model
 Correcting wrong spelling
Note: removal of unwanted characters and extra spaces from the text couldn’t be performed
due to crashing of ram as the dataset is large to be worked upon.
