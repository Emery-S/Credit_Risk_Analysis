# Credit_Risk_Analysis
## Overview: 
This analysis utilizes supervised machine learning algorithms to train, evaluate and make predictions based on patterns present in the data. The purpose is to analyze a data set on credit card credit from the LendingClub. Due to the unbalanced classes expected with credit risk classification the imbalanced-learn and scikit-learn librarys are implimented to evaluate models through resampling. 

For the predictions two oversampling models, RandomOverSampler and SMOTE, as well as an undersampling model, ClusterCentroids, is built along with a combination over and under sampling modle, SMOTEENN algorithm. An ensemble adaBoost classifier and a balanced random forest classifier were also utilized to build potential models for predicting loan risk.

The models mentioned above are evaluated and a recommendation is made regarding the best model to utilize for predicting credit risk.

## Results: 

### Naive Random Oversampling
* The balanced accuracy score is 65%

<img width="321" alt="Screen Shot 2023-03-17 at 8 32 30 PM" src="https://user-images.githubusercontent.com/112206035/226073563-6a2d2f70-5b16-479e-af37-f493d071b8b3.png">

<img width="386" alt="Screen Shot 2023-03-17 at 8 27 30 PM" src="https://user-images.githubusercontent.com/112206035/226073123-9f9e2400-39da-41a7-bb44-ec97ff2c3090.png">

* High_risk precision is around 1% with 62% sensitivity and an f1 of 2%
* Low_risk precision is around 100% with 59% sensitify and an f1 of 74%

<img width="663" alt="Screen Shot 2023-03-17 at 8 27 40 PM" src="https://user-images.githubusercontent.com/112206035/226073160-aeafbc07-025e-44dc-a14d-f41f8ed1a735.png">

### SMOTE Oversampling
* The balanced accuracy score is 66%

<img width="328" alt="Screen Shot 2023-03-17 at 8 33 00 PM" src="https://user-images.githubusercontent.com/112206035/226073600-ed8520c8-0c4d-44d6-b722-c56a2ac23aff.png">

<img width="385" alt="Screen Shot 2023-03-17 at 8 33 15 PM" src="https://user-images.githubusercontent.com/112206035/226073613-b95e8b19-2469-49cd-a662-7802b7c3dfff.png">

* High_risk precision is around 1% with 63% sensitivity and an f1 of 2%
* Low_risk precision is around 100% with 69% sensitify and an f1 of 81%

<img width="653" alt="Screen Shot 2023-03-17 at 8 34 37 PM" src="https://user-images.githubusercontent.com/112206035/226073687-ac2f6377-556c-4510-ab0f-03c0d3e08ed7.png">


## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
