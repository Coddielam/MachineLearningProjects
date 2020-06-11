# MachineLearningProjects
This repository contains some of the data mining projects I conducted on my own. 

## Project Brief:
### Time Series Analysis: Forecasting Walmart Sales with SARIMA and Holt Winters' Expotential Smoothing
Link to Jupyter Notebook:
https://github.com/Coddielam/MachineLearningProjects/blob/master/Time_Series_Walmart_Sales/Time%20Series%20Analysis%20w%20Walmart%20Sales%20EddieLam.ipynb
In this project I applied two classical time series forecasting methods, which both account for trends and seasonalities in time-series data, and they are the Seasonal AutoRegressive Integrated Moving Average and the Holt Winters' Expotential Smoothing. In comparison, the Holt Winters ES approach was the succeeding method and the mean absolute prediction error associated with its predictions is ~3.8%.   

### Titanic Dataset: Learning from Diaster
Link to Jupyter Notebook: (https://github.com/Coddielam/MachineLearningProjects/blob/master/Titanic_Machine_Learning_Project_ChiuMing_Lam.ipynb)
In one of the dataset I explored the Titanic dataset to understand the types of passengers that would most likely survive the ship wreck. Through a series of exploratory analysis and visualizing the data, it becomes quite obvious that the survival of a passenger is largely determined by sex and passenger class/social status. 

### New York Airbnb Unsupervised Learning (Principal Component Analysis)
Link to Jupyter Notebook:
(https://github.com/Coddielam/MachineLearningProjects/blob/master/AirbnbEddie/Airbnb_NewYork_PCA_(Eddie)ChiuMingLam.ipynb)
Many people try to use the New York Airbnb dataset to predict the prices of the listing. However, since the prices of the listings are set by the hosts based on the recommendations from Airbnb's smart pricing system, predicting prices might not be the most sensible analysis. 
When relationships between variables are unclear, it's oftentimes a good idea to explore the variables with unsupervised learning techniques.
In this dataset, I conducted a Principal Component Analysis to identify the factors that set aparts the 5 major neighborhood groups: Brooklyn, Manhattan, Brooklyn, Bronx, Queens, and Staten Island. 


### Predicting Auto Insurance Risk
Link to Jupyter Notebook:
(https://github.com/Coddielam/MachineLearningProjects/blob/master/AutoInsuranceRisk_ChiuMingLam(Eddie).ipynb)
I found this dataset from my business intelligence class's extra coursework section. I assumed the primary usage of the dataset is to predict whether of not a claim applicant's cliam would be accepted or not. Through a series of data visualizing, I came to the hypothesis that one type of claim applicant has the highest claim approval rate -- a young male with stable income and is not married with kids, or more particularly, a young male around 25 of age, who works in the public sector and drives a sports car. 

In the second part of the project I fitted the data with a decision tree and a KNN model. The confusion matrices of the two models revealed that both of them are bad at correctly accepting claims. After some research, it has come clear that the root of the problem comes from the inherent imbalance in the dataset -- most of the claims in the data is rejected and only a tiny portions were accepted. 

To mitigate this problem, I began using Grid Search CV to search for hyperparameters for each the models for the highest auc score. 

The best model identified among all selected is decision tree. However, the decision tree is still appear overly fitted. A potential solution would be to fit a random forest model instead, as it is more robust against overfitting. 
