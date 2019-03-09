# Anomaly-Detection-on-NSL-KDD-dataset

The NSL KDD Dataset is analysed using numpy, pandas,sklearn,matpoltlib and seaborn libraries. 
I have used Jupyter notebook to make the analysis.
Two files are available, the original and RFE and Polynomials. 
The original is an attempt at data analysis to engineer features and to gain an understanding of the relative importance of the features.
Among the machine learning models used include Logistic Regression,  Multinomial Naive Bayes Gaussian Naive-Bayes, MLP Classifier( with (100,)  and (100,100) layersize), Ada Boost Classifier,  Decision Tree Classifier, Random Forest ClassifierGradientBoostingClassifier,Random Forest Classifier.

A summary is given below:

In order to build an effective anomaly detection system, a refined version of the KDD ‘99 Dataset is used as it offers a sizeable amount of features, while being efficient in getting rid of redundancy.
Machine Learning Algorithms are developed to check the effectiveness of Anomaly detection using Python. The relationship between division of labels and effectiveness of the algorithms has been analysed while focusing on Feature Selection and Feature Engineering in order to improve the models. Similar machine learning models are used throughout and f1-scores and accuracy are used as metrics of evaluating the results. However, f1-score(weighted) is given preference as labels are skewed. Analysis is made mainly using Python’s scikitlearn library.

The dataset presents 42 features of which 41 are used as the initial dataset. The features pertain to the connections established with the network, details of information exchanged and information about the errors when they occur during the established connection. In order to establish whether the established connection is an intrusion into the system or a normal connection, the labels have been named “normal” in the case of normal and divided into 4 categories of attack, “DoS”, “Probe”, “R2L”, and “U2R”, each of which then has a different number of sub-categories of attack types.  The method employed is to test the models on (i) the original label types as through Multi-Class Classification , then, (ii) as two- class Classification through labels being replaced as either “Attack” or “Normal”, and, finally, (iii) Multi-class Classification with the labels being divided into 4 sub-categories, and the models being trained on them.

The final method(RFE and Polynomials file) achieved greatest accuracy and f1-scores of all methods.
