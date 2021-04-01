# Customized-Word2Vec
This repository contains additional features, extended to the traditional Word2Vec library, launched in 2013.
This project was part of a larger project that involved sentimental analysis and sarcasm detection. The project details have been added in the repo-description section. 

Directly clone the repository and start using it. The details of how the files are named and strored is given below:-

-> The model made using 3 options - Skipgram model, Common Bag of Words, Negative Sampling.

-> You can change the following model parameters:
* Window Size
* Vector Size
* Learning Rate
* Sub-sampling
* number of epochs you want to train for.

-> Optimizer used is SGD.

-> Other that the main code ipynb, entire training corpus and testing corpus (numpy array) of reuters dataset <b>(ca be downloaded directly from [here]())</b>, I have included an example directory where I have applied my code base.

For more information, please refer to the project report uploaded.

---
## The Example folder contains :

-> The folder contains numpy array of training and testing datasets

-> The folder also contains a pickle file containing the dictionary:
   key - Word (string format)
   values - onehot encoding (numpy array) 

-> Naming Convention of the weight1 files are :

../Window_{window size}/{choice of model}/{learning rate}_{vector size}weight_numpy.npy

These, weight vectors must be dot producted with the onehot vectors to get the actual embeddings in
the format given : W'X { W - Weight ; X - Onehot Vector} 
