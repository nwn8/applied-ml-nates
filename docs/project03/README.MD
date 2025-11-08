# Project 03

## Titanic Data Set - Machine Learning Module 03

Nathan Sloss 11/7/2023

This project will explore three different Machine Learning models:

Decision Tree Classifier (DT) - A Decision Tree splits data into smaller groups based on decision rules (like "is height greater than 150 cm?"). It’s like a flowchart, where each decision point leads to another question until a final classification is reached. Easy to interpret and fast to train, but can overfit if the tree becomes too complex.

Support Vector Machine (SVM) - A Support Vector Machine tries to find the "best boundary" (a hyperplane) that separates data into classes. It works well with complex data and small datasets. Effective when there is a clear margin of separation between classes, but can be computationally expensive for large datasets.

Neural Network (NN) - A Neural Network is inspired by how human brains process information. It consists of layers of interconnected "neurons" that process input data and adjust based on feedback. It can handle complex patterns and non-linear relationships, but needs more data and tuning to avoid overfitting.

## Section 1  Import and Inspect the Data

## Section 2 Data Exploration and Preparation

### 2.1 Handle Missing Values and Clean data

### 2.2 Feature Engineering

## Section 3 Feature Selection and Justification

### 3.1 Choose Features and target 

Case 1: 

input features: alone <br>
target: survived

Case 2:

input features - age<br>
target: survived

Case 3:

input features -  age and family_size <br>
target: survived

### 3.2 Define X features and Y target

### Reflection 3 

Why are these features selected? <br>

It can be assumed that a persons age would have a determining factor on whether they survived the titanic wreck.  <br>

Are there features that are likely to be highly predictive of survival?<br>

According to the correlation matrix earlier, the fare and the pclass have the highest correlation to survivorship.

## Section 4  Train a Classification Model (Decision Tree)


### 4.1 Split the Data


### 4.2 Create and Train a Model (Decision Tree)

### 4.3 Predict and Evaluate Model Performance

### 4.4 Report Confusion Matrix as Heatmap

### Reflection 4

How well did the different cases perform? <br>

Overall the performance was comparable on all 3 decision tree models.  With Case 1 performing the best.  Using the weighted average f-1 score as an overall indicator of performance the range is 0.55 , 0.57 and 0.63 for Case 1 - alone.  <br>

Are there any suprising results? <br>

The recall for the true negatives was very high for Case 2 - age.  While the model did not prove to do very well for true positives.  

Which inputs worked better? Overall age and alone did not have a high correlation to survivorship resulting in low success in the models scores.  Other factors such as pclass and fare would probably be better predictors of survivorship.

## Section 5 Compare Alternative Models (Support Vector C , Neural Network)

### 5.1 Train and Evaluate the Model -- SVC

### Reflection 5

How well did each of these models/cases perform? <br>

Using the weighted average f1 score as the overall indicator of success, The SVC performed very similar to the Decision Tree classifier. Also Case 1 - alone for the SVC model outperformed the other features.  The Neural Network model on Case 3 performed teh best <br>

Are there any suprising results or insights? <br>

The resuls of Case 3 Neural Network were suprising, because using other models the Case 3 did not do very well.  It shows that the model can have just as much of an impact on performance as choosing the correct features<br>

Why might one model outperform the others? I honestly don't know why the Neural Network performed better, but predicted the most correct values out of all of the models.  The SVC performed less well than the Decision Tree most likely due to the low correlation between the survivorship and the features selected.  It may perfom better given more data or using different features. However all models would probably perform better if the features were p_class or fare.



## Section 6 Final thoughts and Insights

1. Summarize Findings - use a table to summarize<br>

Model Type	Case	Features Used	Accuracy	Precision	Recall	F1-Score<br>
Decision Tree	Case 1	Alone	63	64	63	63<br>
----------------Case 2 	Age	61	58	61	55<br>
----------------Case 3	Age + Family Size	59	57	59	57<br>
SMV (RBF Kernel)	Case 1	Alone	63	64	63	63<br>
----------------Case 2 	Age	63	66	63	63<br>
----------------Case 3	Age + Family Size	63	66	63	52<br>
Neural Network	Case  1	Alone				<br>
----------------Case 2 	Age				<br>
----------------Case 3	Age + Family Size	67	66	66	64<br>


2. Discuss Challenges Faced<br>

The overall challenge in picking a classifier model would be in maximizing the results by picking the best features and the best model.  Both will play a factor in producing good results<br>

3. Next steps to gain more insights and/or to explore classification models. <br>

Explore other features and other models to get more accurate predictions.  Perhaps using features that have a higher correlation to survivor rating such as p_class and fare. 