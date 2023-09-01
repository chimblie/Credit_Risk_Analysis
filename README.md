# Credit_Risk_Analysis
1.	Overview of the analysis:
•	The purpose of this analysis is to evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, we imported the  Imbalanced-learn and Scikit-learn as our libraries, then we used the RandomOverSampler and SMOTE algorithms to oversample the data. Then, we used the ClusterCentroids algorithm to undersample the data. 
•	After we resampled the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report. Finally, we used a combinatorial approach of over- and undersampling with the SMOTEENN algorithm to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms. 
2.	Results:
Here is the results of the balanced accuracy scores and the precision and recall scores of all six machine learning models. 
•	RandomOverSampler model
 ![image](https://github.com/chimblie/Credit_Risk_Analysis/assets/121005128/d38556cf-9898-4141-865b-ef6bb695a6d5)

 
The balance accuracy score is about 64%.  The high_risk precision is 1% with 62% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.
•	SMOTE model
 ![image](https://github.com/chimblie/Credit_Risk_Analysis/assets/121005128/37b612af-94e2-42f8-bd7e-b55d07102347)
![image](https://github.com/chimblie/Credit_Risk_Analysis/assets/121005128/95c604fb-c325-49cf-9207-9c2eacf7c8b5)

 
The balance accuracy score is about 64%.  The high_risk precision is 1% with 62% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 65%.
•	ClusterCentroids model
 ![image](https://github.com/chimblie/Credit_Risk_Analysis/assets/121005128/cece5499-937d-46cf-8ae9-fb6a67332cea)

 
The balance accuracy score is about 51%.  The high_risk precision is 1% with 59% sensitivity which makes a F1 of 2% only. Due to the high number of false positives, the low_risk sensitivity is 44%.
•	SMOTEENN model
 ![image](https://github.com/chimblie/Credit_Risk_Analysis/assets/121005128/a546a8f8-b694-43ed-8c39-7d6e86a0ab8c)

The balance accuracy score is about 62%.  The high_risk precision is 1% with 71% sensitivity which makes a F1 of 2% only. Due to the high number of false positives, the low_risk sensitivity is 54%.
•	BalancedRandomForestClassifier model
 ![image](https://github.com/chimblie/Credit_Risk_Analysis/assets/121005128/48f2fd7d-19f7-45a8-b9be-2f53076a0828)
 
The balance accuracy score is about 79%.  The high_risk precision is 4% with 67% sensitivity which makes a F1 of 7% only. Due to the high number of false positives, the low_risk sensitivity is 91%.
•	EasyEnsembleClassifier model
 ![image](https://github.com/chimblie/Credit_Risk_Analysis/assets/121005128/864ef9a5-e009-4aa8-99d5-5fb429f709d6)

The balance accuracy score is about 93%.  The high_risk precision is 7% with 91% sensitivity which makes a F1 of 14% only. Due to the high number of false positives, the low_risk sensitivity is 94%.
3.	Summary:
•	In this project, we evaluated three machine learning models by using resampling to determine which model is better at predicting credit risk. After calculating all the balanced accuracy score, we came to a conclusion that all the model show weak precision in determining if a credit risk is high. For this reason, we would not recommend financial institutions to use any of these models to predict credit risk.
