## Steel Industry Energy Consumption

The information gathered is from the DAEWOO Steel Co. Ltd in Gwangyang, South Korea. It produces several types of coils, steel plates, and iron plates. The information on electricity consumption is held in a cloud-based system. The information on energy consumption of the industry is stored on the website of the Korea Electric Power Corporation (pccs.kepco.go.kr), and the perspectives on daily, monthly, and annual data are calculated and shown.

https://archive.ics.uci.edu/ml/datasets/Steel+Industry+Energy+Consumption+Dataset#


The study consists of two parts:<br>
  (1) Sending the dataframe to the sql server using Pandas library (please see **DF_to_SQL.ipynb**)<br>
  (2) Extracting data from the created sql tables and creating a dataframe using Pandas, cleaning the data (Data preprocessing) and regression analysis (please see **Steel_Industry_Energy_Consumption.ipynb**)<br>

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
    <a>Overview of all features</a><br>
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165169824-d296471e-9760-420b-a689-c56f16fc56db.png">
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165169902-f2ddffbf-8ae9-46d0-b360-2bc0ac4f9ddb.png">
</blockquote>

<a href='#5.0'>Exploratory Data Analysis (EDA)</a><br>
<blockquote>
    <a href='#5.1'>Analyze each feature</a><br>
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165170016-5d38b521-7c78-4d20-9bbf-fbc26150930a.png">
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165170072-5989de93-74ef-4ddf-a3e2-7f2f97ef2049.png">
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165170122-c2bde298-3e73-4ffd-bcfd-772bec38b200.png">
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165170224-cbc2af02-837a-4af5-a540-9def22d6a6dc.png">
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165170424-75dc6b38-8c6b-43ce-94c2-bc70f45f057f.png">
  <br>
    <a href='#5.2'>One Hot Encoding</a><br>
    <a href='#5.3'>Min-Max Scaler</a><br>
    
</blockquote>

<a href='#6.0'>Machine Learning Algorithms and Results</a><br>
<blockquote>
    <a href='#6.1'>Feature engineering</a><br>
    <a href='#6.2'>Correlation of the features</a><br>
    <a href='#6.3'>Split Dataframe</a><br>
    <a href='#6.4'>Building ML models</a><br>
    <blockquote>
        <a>Linear Regression </a><br>
        <a>Decision Tree Regressor</a><br>
        <a>Ridge, Lasso</a><br>
        <a>Gradient Boosting Regressor</a><br>
        <a>Model_Selection - Final</a><br>
      <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165170504-03ed136f-90c5-4d73-910d-0f38561c4fae.png">
    </blockquote>
    <a href='#6.5'>Accuracy improvement of the selected model</a><br>
  <img height="200" alt="image" src="https://user-images.githubusercontent.com/58983814/165170668-f85ec5e9-1a97-4297-ac65-90bd49042bc7.png">
</blockquote>
