# MachineLearningProjects
This repository contains some of the data mining projects I conducted on my own. 

Currently there are two projects in this repository are both of them are in **Jupyter Notebook format**. 

## Project Brief:
### Titanic Dataset: Learning from Diaster
In one of the dataset I explored the Titanic dataset to understand the types of passengers that would most likely survive the ship wreck. Through a series of exploratory analysis and visualizing the data, it becomes quite obvious that the survival of a passenger is largely determined by sex and passenger class/social status. 

### Predicting Auto Insurance Risk
I found this dataset from my business intelligence class's extra coursework section. I assumed the primary usage of the dataset is to predict whether of not a claim applicant's cliam would be accepted or not. Through a series of data visualizing, I came to the hypothesis that one type of claim applicant has the highest claim approval rate -- a young male with stable income and is not married with kids, or more particularly, a young male around 25 of age, who works in the public sector and drives a sports car. 

In the second part of the project I fitted the data with a decision tree and a KNN model. The confusion matrices of the two models revealed that both of them are bad at correctly accepting claims. After some research, it has come clear that the root of the problem comes from the inherent imbalance in the dataset -- most of the claims in the data is rejected and only a tiny portions were accepted. 

To mitigate this problem, I began using Grid Search CV to search for hyperparameters for each the models for the highest auc score. 

The best model identified among all selected is decision tree. However, the decision tree is still appear overly fitted. A potential solution would be to fit a random forest model instead, as it is more robust against overfitting. 
