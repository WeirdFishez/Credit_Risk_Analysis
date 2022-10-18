# Credit_Risk_Analysis


## Overview of the analysis
For this assignemt, we were asked to assist a credit card company in developing a machine learning model that allows them to detect a small percentage of fradulant transactions in their system. In this process we tested 6 different supervised machine learning models and assessed their accuracy in detecting fraud from sample data.

## Results
Accuracy = (TP + TN) / (TP + FP + TN + FN)

Precision = TP/(TP + FP)

Recall/Sensitivity = TP/(TP + FN)

F1/harmonic mean = 2(Precision * Sensitivity)/(Precision + Sensitivity)


### Model: ClusterCentroids
- Balanced Accuracy Score: 0.5103893461611291
- Precision: 0.99
- recall: 0.44

![image](https://user-images.githubusercontent.com/107438816/196526260-c72a45a1-f361-400a-83e3-365d0d09cd28.png)
![image](https://user-images.githubusercontent.com/107438816/196526215-433a1d38-01b2-4c43-af2b-5849bf4bd320.png)
![image](https://user-images.githubusercontent.com/107438816/196526298-fda142b1-16ef-45c4-b213-e20fa54a2f3a.png)



### Model: RandomOverSampler
- Balanced Accuracy Score: 0.6366972052004142
- Precision: 0.99
- recall: 0.65

![image](https://user-images.githubusercontent.com/107438816/196525843-1ac50c94-5c5a-4362-9f7b-ddcd8bff8ab3.png)
![image](https://user-images.githubusercontent.com/107438816/196525890-251d4551-849b-44c4-ab73-6ca561613658.png)
![image](https://user-images.githubusercontent.com/107438816/196525923-a92219b9-ab2c-4afe-bc2c-5b3e8e4e04db.png)


### Model: SMOTE - Oversampling
- Balanced Accuracy Score: 0.6453944426314708
- Precision: 0.99
- recall: 0.66

 ![image](https://user-images.githubusercontent.com/107438816/196525979-2cb2670d-cd1a-4dfa-a383-316fbd0ad47e.png)
 ![image](https://user-images.githubusercontent.com/107438816/196526017-48a64520-c05c-4a33-9b66-79fb60c857e8.png)
 ![image](https://user-images.githubusercontent.com/107438816/196526062-a44bb8d9-4895-4d6a-879d-e279404a1a77.png)



### Model: SMOTEENN - Combination (Over and Under) Sampling
- Balanced Accuracy Score: 0.5103893461611291
- Precision: 0.99
- recall: 0.57

![image](https://user-images.githubusercontent.com/107438816/196529068-21eb0a5d-b1b9-4e1c-bed9-329a272920c0.png)
![image](https://user-images.githubusercontent.com/107438816/196529121-84dcc4d7-0ef5-4d66-a3a9-1b1eda5c6cad.png)
![image](https://user-images.githubusercontent.com/107438816/196529168-260f9660-39b5-4872-9a3f-ce39eff67429.png)


### Model: BalancedRandomForestClassifier
- Balanced Accuracy Score: 0.794967789501674
- Precision: 0.99
- recall: 0.91

![image](https://user-images.githubusercontent.com/107438816/196525015-824808cc-0bcc-45f5-8d65-d49ecdbe09af.png)
![image](https://user-images.githubusercontent.com/107438816/196525256-3d631f5f-954e-4222-8795-e7fe918dafc5.png)
![image](https://user-images.githubusercontent.com/107438816/196525311-84c58315-afb1-4cc6-b104-2ca18ba3d041.png)


### Model: EasyEnsembleClassifier
- Balanced Accuracy Score: 0.7953112472855757
- Precision: 0.99
- recall: 0.90

![image](https://user-images.githubusercontent.com/107438816/196524268-749a2032-2f87-4aaa-b230-eeb071c06eb4.png)
![image](https://user-images.githubusercontent.com/107438816/196524341-28105d50-9a37-47d9-a4d0-ff2b5955351a.png)
![image](https://user-images.githubusercontent.com/107438816/196524417-5ef17d5a-bbc6-48e3-9e7a-400ed507b5e2.png)



## Summary
As can be seen from the outputs above, the most sucessfull models for our credit risk analysis came out to be our Ensemble models BalancedRandomForestClassifier and EasyEnsembleClassifier. All models had a high precision of .99, however this means nothing when they misses the 10-15 true fradulent activities. Therefore We can look to the balanced accuracy score for both models which are leaders with .795. We can also look at the F1 score for both models which is a high .94-.95. This tells us that there is not a pronounced imabalance between sensitivity and precision.
