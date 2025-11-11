# Midterm Project: Classification Analysis

> Author: Nathan Sloss
> Date: 11/11/2025
> Description: This project will test different classification models and features to produce the highest performing machine learning model using the Titanic dataset.



## Dataset

 **Titanic Survival Dataset** (Predict whether a passenger survived the Titanic disaster)
   - [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)


### Titanic Data Set includes the following:<br>

Variable	Definition	Key<br>
survival	Survival	0 = No, 1 = Yes<br>
pclass	Ticket class	1 = 1st, 2 = 2nd, 3 = 3rd<br>
sex	Sex	<br>
Age	Age in years	<br>
sibsp	# of siblings / spouses aboard the Titanic	<br>
parch	# of parents / children aboard the Titanic	<br>
ticket	Ticket number	<br>
fare	Passenger fare	<br>
cabin	Cabin number	<br>
embarked	Port of Embarkation	C = Cherbourg, Q = Queenstown, S = Southampton


Link to notebook: https://github.com/nwn8/applied-ml-nates/blob/main/notebooks/Midterm/classification_NathanSloss.ipynb
Link to peer review: https://github.com/nwn8/applied-ml-nates/blob/main/notebooks/Midterm/peer_review.md


### Conclusion

Comparison of all 3 features : Pclass, Fare, and Aggregate (Agg_squared was not supported for further inquiry), show that Pclass produced the best results in 3 different models Decision Tree, SVC , Neural Network. <br>


Comparing the results of the models for the feature "Pclass" <br>

Decision Tree     <br>
        precision    recall  f1-score   support<br>

           0       0.73      0.83      0.77       110
           1       0.65      0.51      0.57        69

SVC <br>
        precision    recall  f1-score   support

           0       0.73      0.83      0.77       110
           1       0.65      0.51      0.57        69

Neural Network<br>
        precision    recall  f1-score   support

           0       0.73      0.83      0.77       110
           1       0.65      0.51      0.57        69



### NOTE -

 All 3 models produced the same results for the same feature




