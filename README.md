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
* Low_risk precision is around 100% with 59% sensitivity and an f1 of 74%

<img width="663" alt="Screen Shot 2023-03-17 at 8 27 40 PM" src="https://user-images.githubusercontent.com/112206035/226073160-aeafbc07-025e-44dc-a14d-f41f8ed1a735.png">

### SMOTE Oversampling
* The balanced accuracy score is 66%

<img width="328" alt="Screen Shot 2023-03-17 at 8 33 00 PM" src="https://user-images.githubusercontent.com/112206035/226073600-ed8520c8-0c4d-44d6-b722-c56a2ac23aff.png">

<img width="385" alt="Screen Shot 2023-03-17 at 8 33 15 PM" src="https://user-images.githubusercontent.com/112206035/226073613-b95e8b19-2469-49cd-a662-7802b7c3dfff.png">

* High_risk precision is around 1% with 63% sensitivity and an f1 of 2%
* Low_risk precision is around 100% with 69% sensitivity and an f1 of 81%

<img width="660" alt="Screen Shot 2023-03-17 at 8 53 32 PM" src="https://user-images.githubusercontent.com/112206035/226074479-04481d0b-666e-4015-a793-10e603f6b383.png">

### Undersampling: ClusterCentroids
* The balanced accuracy score is 54%

<img width="318" alt="Screen Shot 2023-03-17 at 8 43 29 PM" src="https://user-images.githubusercontent.com/112206035/226074068-b962e681-36c4-4196-84c0-51e08ed05fac.png">

<img width="387" alt="Screen Shot 2023-03-17 at 8 43 50 PM" src="https://user-images.githubusercontent.com/112206035/226074084-74978004-b6d6-4cd1-a309-bce0c641449f.png">

* High_risk precision is around 1% with 69% sensitivity and an f1 of 1%
* Low_risk precision is around 100% with 40% sensitivity and an f1 of 56%

<img width="662" alt="Screen Shot 2023-03-17 at 8 44 02 PM" src="https://user-images.githubusercontent.com/112206035/226074092-f8f5d336-7bcb-480c-afd1-b37e0648bc6b.png">

### Combination (Over and Under) Sampling: SMOTEENN 
* The balanced accuracy score is 65%

<img width="317" alt="Screen Shot 2023-03-17 at 8 45 00 PM" src="https://user-images.githubusercontent.com/112206035/226074123-3cc07af9-7b0d-46ae-b430-106b853f425f.png">

<img width="391" alt="Screen Shot 2023-03-17 at 8 46 30 PM" src="https://user-images.githubusercontent.com/112206035/226074184-166b90de-a878-42af-a899-63b104412149.png">

* High_risk precision is around 1% with 72% sensitivity and an f1 of 2%
* Low_risk precision is around 100% with 57% sensitivity and an f1 of 73%

<img width="656" alt="Screen Shot 2023-03-17 at 8 46 49 PM" src="https://user-images.githubusercontent.com/112206035/226074204-c50fbb4c-1fe7-45b3-9146-093a134233b9.png">

### Balanced Random Forest Classifier
* The balanced accuracy score is 79%

<img width="315" alt="Screen Shot 2023-03-17 at 8 48 12 PM" src="https://user-images.githubusercontent.com/112206035/226074248-e15eeedb-5ac5-4301-8fad-c6eeca1c44f6.png">

<img width="387" alt="Screen Shot 2023-03-17 at 8 48 27 PM" src="https://user-images.githubusercontent.com/112206035/226074261-c1c3bbd0-a6f6-4eae-af84-cb77681cf669.png">

* High_risk precision is around 3% with 70% sensitivity and an f1 of 6%
* Low_risk precision is around 100% with 87% sensitivity and an f1 of 93%

<img width="663" alt="Screen Shot 2023-03-17 at 8 53 51 PM" src="https://user-images.githubusercontent.com/112206035/226074493-287463e2-a5c5-4c13-a1a9-f8f1a20c6db1.png">

### Easy Ensemble AdaBoost Classifier
* The balanced accuracy score is 93%

<img width="324" alt="Screen Shot 2023-03-17 at 8 50 15 PM" src="https://user-images.githubusercontent.com/112206035/226074343-ddc21997-54cd-4551-9fd7-fe553830ec42.png">

<img width="387" alt="Screen Shot 2023-03-17 at 8 50 50 PM" src="https://user-images.githubusercontent.com/112206035/226074368-14551dd5-e056-4e50-a32f-956475ef000f.png">

* High_risk precision is around 9% with 93% sensitivity and an f1 of 16%
* Low_risk precision is around 100% with 94% sensitivity and an f1 of 97%

<img width="661" alt="Screen Shot 2023-03-17 at 8 54 18 PM" src="https://user-images.githubusercontent.com/112206035/226074512-6b1619e8-5417-437f-b059-f441d2d6aef5.png">

## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
