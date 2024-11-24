

# Neural Network Classification of Mushrooms as either Poisonous or Edible
CS577/CS549 Final project double feature

Many people forage for mushrooms for consumption, recreational purposes, and monetary purposes. Our research holds practical real world value in helping people assess which mushrooms are safe to ingest based on morphological information and habitat information. We aim to create a tool which will sort through a large volume of these metrics in order to identify poisonous varieties of mushrooms belonging to the Agaricus and Lepiota families. Given that we are looking at whether any particular mushroom is edible or not and having a large number of features, our dataset pushed us towards constructing a neural network. Biologically speaking, before constructing the machine learning approach, we cannot expect any strong indicators within morphological features due to edible mushrooms often copying the appearance of poisonous mushrooms in order to ward off predation. We will construct a neural network using TensorFlow and assess how adding additional layer types, like different normalization layers or batch layers, affect the accuracy of the model.

## Dataset Description
The UC Irvine’s mushroom data consists of 3.12 million data entries (before we cut away NAs). Before data cleaning there are 21 features, mostly categorical with a few quantitative features such as stem length/diameter, and cap diameter. Some features have an unacceptable amount of missing records, so we believe that removing the 5 fields with [null] data percentage of over 40 to be justified. The rest of the data will have records with any NAs purged, resulting in a theoretical loss of around 1.25 million records. This would then leave us with 1.87 million individuals, which should be enough for us to run analyses on. 

https://www.kaggle.com/datasets/davinascimento/poisonous-mushrooms


## Models to be Used
We chose to apply a neural network model for our project on distinguishing between edible and poisonous mushrooms. With our dataset consisting of various features of mushroom classifications, a neural network model would allow us to use these features as inputs to train the model. We chose to use a neural network for its built in feature selection capabilities.

## Evaluation Metrics
Our primary evaluation metrics we plan on using are accuracy and F1-score, which will also effectively encapsulate the precision and recall as well. When using neural nets these metrics seem to be the standard at best conveying the quality of our models.

