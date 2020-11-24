# Churn Prediction (Telecom company)
You can see fancy html-version [here](https://nbviewer.jupyter.org/github/paperchampion/DLS_20-21/blob/master/simple-churn-prediction/simple-churn-prediction.ipynb)

In this task teachers split [this dataset](https://www.kaggle.com/blastchar/telco-customer-churn) (presumably) in the following proportions: ~75% for train set (train.csv), ~25% for test set (test.csv) – and hosted [Kaggle InClass competition](https://www.kaggle.com/c/advanced-dls-fall-2020/overview). Task requirements were quite simple (see [baseline.ipynb](https://github.com/paperchampion/DLS_20-21/blob/master/simple-churn-prediction/baseline.ipynb)):
* Download datasets (you can find it [here](https://drive.google.com/drive/folders/1JimvXHOwXeD-4PTeRNvoev1jbZLI6FJW)) and detect "missing" values;
* Make simple EDA (just feature visualisation);
* Preprocessing or making a pipeline;
* Building a linear model (preferably logistic regression);
* Building a gradient boosting model (preferably Catboost);
* Making final predictions on the test set and submission on Kaggle.  
Evaluation metric is `AUC – ROC`, baseline score – 0,84. As you see on the [leaderboard](https://www.kaggle.com/c/advanced-dls-fall-2020/leaderboard), it's pretty simple to beat the score. Also, data is really clean, without all these bunches of NaN values, outliers and anomalies. Nice dataset, so to say.   

I've decided to make this homework more complex and involve other ML methods/techniques into it. Below, there will be a sort of tasklist with completed and upcoming steps.

1. Data Cleansing:
  - [x] Find empty values and replace them with zero;
    - [ ] Try other replacing methods (e.g. KNN)
  - [x] Find duplicates(open to question) and delete them;
    - [ ] Make a rough probability estimation: could it be a coincidence?
2. EDA:
  - [x] Numeric features analysis;
    - [ ] Generate new features based on nonlinear transformations;
    - [ ] Find a solution of outliers-problem;
  - [x] Categorical features analysis;
    - [x] Drop useless features
3. Pipelines and validation:
  - [x] Make a simple cross-validation;
    - [ ] Try other validation schemes; probably, estimate the optimal number of folds;
  - [x] Build a simple pipeline;
    - [ ] Try other numeric and categorical transformers;
4. Building models:
  - [x] Build baseline models: logreg, random forest, xgboost, Catboost;
  - [x] Primitive hyperparameters tuning
  - [ ] More complex hyperparameters tuning
  - [ ] Try ensemble methods, and just for fun, neural networks
  - [ ] Try sampling techniques
  - [ ] FP/FN predictions analysis
5. General tasks:
  - [x] Adapt seaborn methods to the latest release;
  - [ ] Adapt notebook for submitting on kaggle
