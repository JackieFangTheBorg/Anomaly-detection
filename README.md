## This project is a part of Coursera's "Machine learning course by Andrew Ng". About 50-60 % of the code was provided by coursera.

### OBJECTIVE: 
To build an algorithm to detect failing servers (anomalous behavior) in a network of computers.

### APPROACH: 
Fit a Gaussian model to data, and detect data points with low probabilities as anomalies.

### METHODOLOGY: 

### STUDYING INPUT DATA:
The input data constitutes two features: throughput (Mb/s) and latency of response(ms) for  307 unlabeled examples. 

### CALCULATE GAUSSIAN PARAMETERS:
Calculate mean and variance of each feature. Estimate probability distribution of all data points in the training data set. 

### SELECT THRESHOLD:
If the probability value of a data point is less than a threshold value, it is determined as an anomaly. The threshold is selected by iterating through a set of values and selecting the one that yields the best F1 score on the cross-validation set (labeled examples). 

### RESULT:
A model that can detect anomalous behavior in a network of computers has been built. This model is not constrained by the dimension of the data. Hence the same model can be trained on datasets with additional features and can be used to detect anomalies in the high dimensional dataset. The detected anomalies are marked in red as shown below.

![ANOMALY DETECTION](https://github.com/thiagunagu/Anomaly-detection/raw/master/anomaly.jpg)

### APPENDIX:

Attached files: 
ex8 – Anomaly detection model
estimateGaussian-Function to calculate mean, variance, and estimate Gaussian distribution
SelectThreshold-Function to select threshold value

### FORMULAE:

![FORMULAE](https://github.com/thiagunagu/Anomaly-detection/raw/master/Formulas.JPG)
