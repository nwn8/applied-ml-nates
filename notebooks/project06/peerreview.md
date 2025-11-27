### Review

Link to repository
[https://github.com/hasherlaws18/applied-ml-houstonasherlaws/blob/main/notebooks/Final/ml_regression_HoustonAsherLaws.ipynb]<br><br>

Clarity & Organization (Is the notebook structured and easy to follow?)<br><br>

Yes, very nice job organizing and easy to follow<br><br>


Feature Selection & Justification (Do the chosen features make sense given the objectives?)<br><br>

Yes he chose the Lot size, year sold, and month sold  as his feaztures.  given the objective of predicting Sale price these are good choices.  Although there are 81 columns in his data set, he could have chosen many more features or entirely different ones.  

Model Performance & Comparisons (Are the results and comparisons clearly explained?)<br><br>

I don't think the models performed well.  <br>

- R² values: All are very low. Even the best (0.138) means the model explains only ~13.8% of the variance. That’s weak predictive power.<br>
- Error metrics (RMSE, MAE): Pipeline 2 reduces both RMSE and MAE compared to baseline, but the improvement is modest (~3–4%).<br>
- Scaling impact: Pipeline 1 shows no improvement because scaling doesn’t change linear regression’s fit when features are already comparable scales.<br>
- Polynomial features: Pipeline 2 did help slightly, but the gain is small relative to the error magnitude.<Br><br>


Reflection Quality (Are insights well thought out?)<br>

Its interesting because his features didn't really provide much insight but it was perfect for the pipeline method.  Pipelines seem to work well on data that doesn't have a strong relationship to the target variable or where data is missing.  Although the results are poor compared to other features, they prove that pipelines work. 

