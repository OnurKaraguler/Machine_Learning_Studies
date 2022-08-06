## AI4I 2020 Predictive Maintenance Dataset Data Set

Since real predictive maintenance datasets are generally difficult to obtain and in particular difficult to publish, we present and provide a synthetic dataset that reflects real predictive maintenance encountered in industry to the best of our knowledge.

The study consists of:<br><br>
<a href='#1.0'>Functions to be used</a><br>
<blockquote>
    <a>Pandas</a><br>
    <a>Visualization</a><br>
    <a>Confusion matrix and metrics</a><br>
    <a>Encoding</a><br>
    <a>KBinsDiscretizer</a><br>
    <a>Scaler (Standard, MinMax)</a><br>
    <a>Missing value imputation</a><br>
</blockquote>
<a href='#2.0'>Import Libraries</a><br>
<a href='#3.0'>Load Data</a><br>
<a href='#4.0'>Exploratory Data Analysis (EDA)</a><br>
<blockquote>
    <a href='#4.1'>Analyze each feature</a><br>
<img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/183268106-e1dba10f-662d-44b9-b712-120d9a954618.png"> <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/183268114-a95859dc-5b4b-428c-9e14-83f2bd9247a3.png"> <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/183268121-1495a834-4f44-4792-8918-c841f85d091d.png">

<a href='#5.0'>Machine Learning Algorithms and Results</a><br>
<blockquote>
    <a href='#5.1'>Feature engineering</a><br>
      <blockquote>
        <a>Check categorical columns</a><br>
        <a>Constant and quasi constant features removal</a><br>
        <a>Remove duplicate features</a><br>
        <a>Drop highly correlated features using Pearson Correlation</a><br>
        <a>SelectFromModel using Logistic Regression</a><br>
        <a>GenericUnivariateSelect and ANOVA F-value</a><br>
        <a>SelectKBest and Mutual Information</a><br>
        <a>RFE (Recursive feature elimination)</a><br>
    </blockquote>
    <a href='#5.2'>Correlation of the features</a><br>
      <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/183268213-e1985093-6314-4e6c-b311-53327dc248e5.png"><br>
    <a href='#5.3'>Split Dataframe</a><br>
    <a href='#5.3'>Overcoming Class Imbalance using SMOTE</a><br>
      <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/183268242-3ad11a2a-d37c-4146-9802-3ed383a35624.png"><br>
    <a href='#5.4'>Building ML models</a><br>
    <blockquote>
        <a>Logistic Regression </a><br>
        <a>Random Forest</a><br>
        <a>Naive Bayes</a><br>
        <a>SVM</a><br>
        <a>Stochastic Gradient Descent</a><br>
        <a>Gradient Boosting Trees</a><br>
        <a>xgboost - XGBClassifier</a><br>
        <a>Model_Selection - Final</a><br>
      <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/183268297-3f24d284-73d5-450b-b10b-bba5460e440d.png">
    </blockquote>
    <a href='#5.5'>Evaluation of the selected model</a><br>
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/183268365-7b40655b-c77b-4e34-9504-1b2a453ecfdc.png">
</blockquote>
