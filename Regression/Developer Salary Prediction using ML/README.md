## Developer Salary Prediction using Machine Learning

The purpose of the study is to predict of annual salaries ($) of professional software developers who know Python. Data from the Developer Survey conducted by Stack Overflow in 2020 and attended by 65,000 people were used in this analysis. 

https://insights.stackoverflow.com/survey/2020#overview

<img width="257" alt="image" src="https://user-images.githubusercontent.com/58983814/124835864-ab753c00-df8a-11eb-8b58-93df8ddaaad8.png">

The study consists of two parts:<br>
  (1) Creating data frames from the  survey data and sending them to the sql server using Pandas library (please see **df_to_sql.ipynb**)<br>
  (2) Extracting data from the created sql tables and creating a dataframe using Pandas, cleaning the data (Data preprocessing) and regression analysis (please see **salary_prediction.ipynb**)<br>

<ul>
<li>Bar, histogram and scatter plots have been created with Matplotlib for data visualization. Missing values in the dataframe have been plotted using the heatmap created with Seaborn.</li>

<img height="150" src="https://user-images.githubusercontent.com/58983814/124914364-ef068f00-dff8-11eb-93ae-ba4215809170.png"> <img height="150" src="https://user-images.githubusercontent.com/58983814/124914521-1e1d0080-dff9-11eb-830f-00ad982f5a3e.png"> <img height="150" src="https://user-images.githubusercontent.com/58983814/124914615-3ab93880-dff9-11eb-903f-d5840c5cd0cd.png"> <img height="150" src="https://user-images.githubusercontent.com/58983814/124914732-5e7c7e80-dff9-11eb-8ca1-44ae68bef5e6.png">

<li>Missing values in the 'YearsCodePro' and 'ConvertedComp' columns have been predicted using Random Forest Classifier.</li>
<li>Features that are highly correlated to each other have been removed from the dataframe to simplify the model and increase efficiency.</li>
<li>Outliers have been dropped using boxplot created with Matplotlib.</li>
<img height="75" src="https://user-images.githubusercontent.com/58983814/124918209-7229e400-dffd-11eb-9fce-6cd013c11cec.png">
<li>Linear Regression, PolynomialFeatures, Decision Tree, Ridge, Lasso and GradientBoostingRegressor machine learning algorithms have been applied and compared with R2 (coefficient of determination) and RMSW (Root Mean Square Error) metrics. Based on the results of the metrics, GradientBoostingRegressor has been chosen.</li>
<li>Some data causing unsuitable residuals have been removed from the dataframe. Thus, the Accuracy (R2) of the regression model has been improved from 63% to 83%.</li>
</ul>

![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) **RESULT:** When the information below is given, annual salary of a professional software developer can be predicted with 83% probability.
<ul>
<li><strong>YearsCodePro</strong> -> NOT including education, how many years have you coded professionally (as a part of your work)?</li>
<li><strong>Country</strong> -> Where do you live?</li>
<li><strong>OpSys</strong> -> What is the primary operating system in which you work?</li>
<li><strong>OrgSize</strong> -> Approximately how many people are employed by the company or organization you currently work for?</li>
</ul>

