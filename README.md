# Contributions & Team Members
- Sri Sethu Madhavan S
- Harshavardhan M V
- Shrihari A

# Introduction
  Phishing has emerged as a major problem in the rapidly changing digital 
landscape as a result of the rise in internet usage. Phishing is the act of deceiving 
individuals into clicking on fraudulent links that take them to malicious websites, 
allowing confidential information to be collected without the user's awareness. 
Phishing URLs are difficult to recognize using pattern matching because they 
frequently use strategies like misspelled words, phony subdomains, or character 
changes to evade detection. Phishing URLs could seem safe at first, but after a while 
they might lead people to unsafe websites. In this work, phishing URLs are detected 
by feature extraction and then applied to specific algorithms using machine learning 
methods like Random Forests, Decision Trees, Light GBM, Logistic Regression, and 
Support Vector Machine (SVM). 

# Dataset Description
  - Dataset for Phishing URL: Phishing URLs were collected from a service called Phish Tank, an open-source service.
  - Dataset for Benign URL: University of New Brunswick and the number of legitimate URLs in that dataset is around 35000.


# Architecture
![image](https://github.com/project-ssh/Machine-Learning/assets/174055041/55857ba7-cab0-402b-a2c0-3bfc7e78904c)

# Methodology
The methodology used in the study involves the application of machine learning algorithms for detecting malicious URLs, data preprocessing, feature extraction using lexical domain-based features, and the application of machine learning models to the extracted features.

# Features
The Initial Features extracted from the URL are
- Have_IP
- Have_At
- URL_Length
- URL_Depth
- Redirection
- https_Domain
- Prefix/Suffix
- Domain_Age
- Domain_End
- Subdomain_Count
- DNS_Record
- Web_Traffic 
- Tiny_URL
- Statistical Report

# Boruta Feature Selection Algorithm
The Boruta feature selection algorithm identifies important features by leveraging a random forest classifier. It starts by creating shadow features, which are shuffled duplicates of the original features. The dataset, now containing both original and shadow features, is used to train a random forest model. The importance scores of the original features are then compared to the highest importance scores of the shadow features. If an original feature's importance score is significantly higher than the shadow features, it is deemed important; if lower, it is considered unimportant. Features with unclear importance are tentatively kept for further testing, ensuring a robust selection of relevant features.

# Machine Learning Algorithms
The Machine Learning Algorithms used are
  - Decision Tree Classifier
  - Random Forest Classifier
  - Logistic Regression
  - LightGBM
  - Support Vector Machine

# Results
  ![image](https://github.com/project-ssh/Machine-Learning/assets/174055041/49492663-1ca1-4aae-93eb-50a7370b777c)

