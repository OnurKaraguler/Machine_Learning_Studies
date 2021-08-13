## Customer Churn Analysis

This data set contains details of a bank's customers and the target variable is a binary variable reflecting the fact whether the customer left the bank (closed his account) or he continues to be a customer.

The study consists of:<br>
  (1) Importing Libraries<br>
  (2) Loading the data<br>
  <ul>
      <li>created dataframes by reading cvs files with Pandas</li>
      <li>checked whether the dependent variable is balanced or imbalanced.</li>
          <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/128782908-8fff5875-1094-4754-9e9d-65d7ad01dbd8.png">
      <li>checked for missing values</li>
  </ul>
  
  (3) Data Preprocessing<br>
      <ul>
        <li>[3.1 Functions to be used](#31)</li>
            <ul>
              <li>Visualizations</li>
                  <ul>
                    <li>stacked_bar_chart: plot a stacked bar chart to show how a feature is categorized using the independent feature</li>
                    <img height="100"  alt="image" src="https://user-images.githubusercontent.com/58983814/128782985-610590b2-ede2-403a-b4b7-d479aa5c2e85.png">
                    <li>histogram: plot a histogram to show how a continuous variable is distributed</li>
                    <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/128783759-2abbf071-3539-43e0-ae61-028c6279f60d.png">
                    <li>box_plot: plot a boxplot to show how the values in the dataset are spread out</li>
                    <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/128783086-d21c7b97-6bc1-474f-964f-631d7634da57.png">
                  </ul>
            </ul>
            <ul>
              <li>Encoding </li>
              <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/127749099-7ab7e089-9504-45f9-b4dd-33f9a9103834.png">
                  <ul>
                    <li>ohe_to_df: One Hot Encoding-find the unique values per feature and transform the data to a binary one-hot encoding</li>
                    <li>encode_categorical_column: Convert each value in a categorical column to a number from 0 to the number of items-1 by encoding</li>
                  </ul>
            </ul>
            <ul>
              <li>KBinsDiscretizer </li>
                  <ul>
                    <li>is used to convert a continuous data into categorical data</li>
                  </ul>
            </ul>
            <ul>
              <li>Standardization (StandardScaler)  </li>
                  <ul>
                    <li>transform(scale) the mean of a feature to be 0 and the standard deviation to be 1</li>
                  </ul>
            </ul>
        <li>[3.2 Analyze each feature](#32)</li>
              <ul>
                <li>Each feature examined in depth using related visualization functions</li>
                <li>Encoded</li>
                <li>Dropped outliers and standardised</li>
              </ul>
        <li>[3.3 Feature engineering](#33)</li>
            <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/127749043-f5b849f7-1f48-4f5b-bfff-300f6a21aa62.png">
              <ul>
                <li>removed the features that they have at least 99% same value</li>
                <li>removed duplicate features </li>
                <li>dropped highly correlated features using Pearson Correlation</li>
                <li>first feature elimination done with SelectFromModel according to their importance assigned by logistic regression</li>
                <li>best features selected with Univariate feature selection (GenericUnivariateSelect and SelectKBest) based on univariate statistical tests (ANOVA F-value and Mutual Information)</li>
              </ul>
          <li>[3.4 Correlation of the features](#34)</li>
                <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/128784061-72c06d3e-5be4-4198-bb5d-bed45bdbf003.png">
      </ul>
  (4) Machine Learning Algorithms and Results<br>
      <ul>
        <li>[4.1 Overcoming Class Imbalance using SMOTE](#41)</li>
            <ul>
              <li>It is an imbalanced data where the target variable, churn has 79.7% customers not churning and 20.3% customers who have churned</li>
              <li>SMOTE: Synthetic Minority Oversampling Technique will be used for creating synthesized data</li>
              <li>A comparative analysis will be done on the dataset using RandomForestClassifier</li>
              <li>The accuracy metric will be ignored to evaluate the performance of the classifier on this imbalanced dataset</li>
              <li>Precision, recall, F1-score metrics will be taken into account</li>
            </ul>
          <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425118-9c6366be-999a-4eac-b14a-d5cb865b5124.png">
        <li>[4.2 Building ML models ](#41)</li>
            <ul>
              <li>Logistic, Random Forest, Naive Bayes, Support Vector Classification, k-Nearest Neighbours, Stochastic Gradient Descent, Gradient Boosting Trees, xgboost -> XGBClassifier</li>
            </ul>
        <li>[4.3 Model selection - final](#42)</li>
              <ul>
              <li>best model selected according to the accuracy</li>
                <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425219-99bfe891-5871-4b97-8ac5-4b5da86f764e.png">
            </ul>
        <li>[4.4 Evalueation of the selected model](#43)</li>
              <ul>
              <li>computed and visually represented confusion matrix to evaluate the accuracy of a classification</li>
                <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425271-bdfd6fd2-21fb-4e0d-b0f0-bbafc9647342.png"> <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425292-0561162f-1597-4a40-9730-027b61bb91cf.png">
              <li>Graphs for threshold determination</li>
                    <ul>
                      <li>ROC & AUC</li>
                      <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425350-862d8257-d051-4dc3-a38c-3b58baed7f29.png">
                      <li>TPR & TNR - Threshold </li>
                      <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425381-4171b3df-9ab3-4c9f-a361-6f7091b37cba.png">
                      <li>Precision(PPV) & NPV - Recall</li>
                      <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425404-94b473d6-7ea6-4c87-9578-ae2bd23c1697.png">
                      <li>Accuracy - Threshold</li>
                      <img height="150" alt="image" src="https://user-images.githubusercontent.com/58983814/129425420-7ac745f6-3877-4b65-93e1-b06ad78ffe05.png">
                    </ul>
            </ul>
      </ul>
