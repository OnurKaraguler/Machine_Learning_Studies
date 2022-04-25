## House Prices - Advanced Regression Techniques

Ask a home buyer to describe their dream house, and they probably won't begin with the height of the basement ceiling or the proximity to an east-west railroad. But this playground competition's dataset proves that much more influences price negotiations than the number of bedrooms or a white-picket fence.

With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this competition challenges you to predict the final price of each home.

Goal: It is your job to predict the sales price for each house. For each Id in the test set, you must predict the value of the SalePrice variable.

Metric: Submissions are evaluated on Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted value and the logarithm of the observed sales price. (Taking logs means that errors in predicting expensive houses and cheap houses will affect the result equally.)

https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques


The study consists of two parts:<br>
  (1) Sending the survey dataframe to the sql server using Pandas library (please see **df_to_sql.ipynb**)<br>
  (2) Extracting data from the created sql tables and creating a dataframe using Pandas, cleaning the data (Data preprocessing) and regression analysis (please see **House_Prices.ipynb**)<br>

<a href='#1.0'>Functions to be used</a><br>
<blockquote>
    <a>Pandas</a><br>
    <a>Visualization</a><br>
    <a>Encoding</a><br>
    <a>Scaler (Standard, MinMax)</a><br>
</blockquote>

<a href='#2.0'>Import Libraries</a><br>
<a href='#3.0'>Connect to the mysql database</a><br>
<blockquote>
    <a>Establish a connection to SQL Database</a><br>
</blockquote>

<a href='#4.0'>Load Data</a><br>
<blockquote>
    <a>Query the database table into a dataframe</a><br>
</blockquote>

<a href='#5.0'>Exploratory Data Analysis (EDA)</a><br>
<blockquote>
    <a href='#5.1'>Split dataframe with/without missing values</a><br>
    <a href='#5.2'>Preprocessing for the dataframe without missing values</a><br>
    <a href='#5.3'>Preprocessing for the dataframe with missing values</a><br>
    <a href='#5.4'>Save the preprocessed dataframe and load it again</a><br>
</blockquote>

<a href='#6.0'>Machine Learning Algorithms and Results</a><br>
<blockquote>
    <a href='#6.1'>Feature engineering</a><br>
    <a href='#6.2'>Correlation of the features</a><br>
    <a href='#6.3'>Save the dataframe with selected features and load it again</a><br>
    <a href='#6.4'>Split Dataframe</a><br>
    <a href='#6.5'>Building ML models</a><br>
    <blockquote>
        <a>Linear Regression </a><br>
        <a>Decision Tree Regressor</a><br>
        <a>Ridge, Lasso</a><br>
        <a>Gradient Boosting Regressor</a><br>
        <a>Model_Selection - Final</a><br>
    </blockquote>
    <a href='#6.6'>Accuracy improvement of the selected model</a><br>
</blockquote>

<a href='#7.0'>Submission</a><br>
<blockquote>
    <a>Results on the Kaggle website</a><br>
</blockquote>
