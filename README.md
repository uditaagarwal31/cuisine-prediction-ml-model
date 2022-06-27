# cuisine-ml-model

What if you wanted to determine whether a given cuisine was likely to use fenugreek? What if you wanted to see if, given a present of a grocery bag full of star anise, artichokes, cauliflower, and horseradish, you could create a typical Indian dish? 

This cuisine recommendation machine learning model predicts a given national cuisine based on a group of ingredients using the Linear SVC Classification Model. The dataset used is cuisines.csv which contains 380 ingredients. 

In the clean_data.ipynb notebook, the data is cleaned and balanced. The distribution of data is examined and recurrent data is cleaned. Using Synthetic Minority Over-sampling Technique (SMOTE), the data is balanced to gain better results during classification. This cleaned data is saved in cleaned_cuisines.csv.

In the classification_models.ipynb notebook, the cleaned dataset is used with a variety of classifier algorithms to predict a given national cuisine based on a group of ingredients. The classifiers used are Logistic Regression, Linear SVC Classifier, K-Neighbors Classifier, and Support Vector Classifier. For all these classifiers, the data is split into testing and training groups and the models are trained. The reports are printed and their accuracies are compared to decide which technique should finally be used to build the cuisine recommendation model. 

In the cuisine_recommender_model.ipynb notebook, the SVC Classification model is built using the cleaned dataset to build the cuisine recommendation model. It is converted to Onnx to enable developers to use it in a variety of different frameworks and tools.
