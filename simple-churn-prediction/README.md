# Churn Prediction (Telecom company)
In this homework teachers split [this dataset](https://www.kaggle.com/blastchar/telco-customer-churn) (presumably) in the following proportions: ~75% for train set (train.csv), ~25% for test set (test.csv) – and hosted [Kaggle InClass competition](https://www.kaggle.com/c/advanced-dls-fall-2020/overview). Task requirements were quite simple (see [baseline.ipynb](https://github.com/paperchampion/DLS_20-21/blob/master/simple-churn-prediction/Baseline.ipynb)):
* Download datasets (you can find it [here](https://drive.google.com/drive/folders/1JimvXHOwXeD-4PTeRNvoev1jbZLI6FJW)) and detect "missing" values;
* Make simple EDA (just feature visualisation);
* Preprocessing or making a pipeline;
* Building a linear model (preferably logistic regression);
* Building a gradient boosting model (preferably Catboost);
* Making final predictions on the test set and submission on Kaggle.  
Evaluation metric is `AUC – ROC`, baseline score – 0,84. As you see on the [leaderboard](https://www.kaggle.com/c/advanced-dls-fall-2020/leaderboard), it's pretty simple. Also, data is really clean, without all these bunches of NaN values, outliers and anomalies. Nice dataset, so to say.   

I've decided to make this homework more complex and involve other methods/techniques into it. Below, there will be a sort of tasklist with completed and upcoming steps. I'll update it a little later, I promise.


- [x] Spam
- [x] Ham
- [ ] Spam and ham
