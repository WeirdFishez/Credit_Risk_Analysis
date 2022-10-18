# Credit_Risk_Analysis


## Overview of the analysis
Explain the purpose of this analysis.

## Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

Accuracy = (TP + TN) / (TP + FP + TN + FN)


### Model: ClusterCentroids
- Balanced Accuracy Score: 0.5103893461611291
- Precision: 0.99
- recall: 0.44

### Model: RandomOverSampler
- Balanced Accuracy Score: 0.6366972052004142
- Precision: 0.99
- recall: 0.65

### Model: SMOTE - Oversampling
- Balanced Accuracy Score: 0.6453944426314708
- Precision: 0.99
- recall: 0.66

### Model: SMOTEENN - Combination (Over and Under) Sampling
- Balanced Accuracy Score: 0.5103893461611291
- Precision: 0.99
- recall: 0.57

### Model: BalancedRandomForestClassifier
- Balanced Accuracy Score: 0.794967789501674
- Precision: 0.99
- recall: 0.90

![image](https://user-images.githubusercontent.com/107438816/196523939-e3a5471d-72a8-48fa-b34e-dca11c2fa98e.png)
![image](https://user-images.githubusercontent.com/107438816/196524131-f640ddc5-29ef-47ef-be97-0b69f819322c.png)
![image](https://user-images.githubusercontent.com/107438816/196524586-c1a20742-e4b1-4721-88aa-a78f8204f883.png)




### Model: EasyEnsembleClassifier
- Balanced Accuracy Score: 0.7953112472855757
- Precision: 0.99
- recall: 0.89

![image](https://user-images.githubusercontent.com/107438816/196524268-749a2032-2f87-4aaa-b230-eeb071c06eb4.png)
![image](https://user-images.githubusercontent.com/107438816/196524341-28105d50-9a37-47d9-a4d0-ff2b5955351a.png)
![image](https://user-images.githubusercontent.com/107438816/196524417-5ef17d5a-bbc6-48e3-9e7a-400ed507b5e2.png)



## Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
