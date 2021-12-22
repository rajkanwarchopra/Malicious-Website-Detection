# Malicious-Website-Detection

Team : Prabhnoor Singh, Ojasvi Sharma, Rajkanwar Chopra

## OBJECTIVE

Build a system to classifiy a url as malicious or safe using machine learning.

## DATASET


* Initially the URLs alongwith Phishing tags were downloaded from: https://www.kaggle.com/simsek/openphishcom-phishing-urls-on-oct-2-2017#dataset.csv
* Many useful parameters (URL-based features, Domain-based features, Page-based features and Content-based features) were extracted using web scraping and some basic computations : [makeDataset.py] (for the code), [dataset.csv]
* Dataset after preparation and pre-processing: [final_cleaned_dataset.csv] 

## Pre-Processing

* Cleaning: Missing-values by imputation, domain-knowledge, Mean-Mode substitutions and other techniques
* Merging and Joining of datasets
* Standardization of numerical features
* Analysis: Graphs(1-D,2-D,3-D,n-D)




## ML
### K-Nearest Neighbors
* Train data + Cross Val data -> 70%
* kd-tree algorithm for finding optimal-k (for better time performance)
* Accuracy on unseen test data: 94.86%
* Confusion Matrix (Without optimization):


### Observations
*Kd-tree time complexity

  -> When d (number of features) is small : O(log (n))
  
  -> When d is not small : O(2^d (log (n)))
  
* K-NN interpretibility decreases as dimensionality increases
* K-NN uses Minkowski Distance ( esp. Euclidean distance) which fails in higher dimensions
* #### Curse of Dimensionality [https://en.wikipedia.org/wiki/Curse_of_dimensionality]

  -> Hughes Phenomenon
  
  -> As d increases Overfitting increases (generally)
  
  -> Distance functions (Euclidean)
  


### Genetic Algorithms and Bio-inspired algos
* As TSNE and PCA does not account for the output label while dimensionality reduction, other techniques would be more suitable
* This algorithm short-listed only 7 features (major reduction)
* Thus, simplifying time complexity for productionazing as well as reducing the dimensionality
* Accuracy: 96.89%
* [Code](https://github.com/philipkalinda/GeneticFS/blob/master/geneticfs/algorithm.py)  







