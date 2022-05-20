## Customer Churn Analysis

- Customer churn analysis is important in terms of identifying old customers without loss and making new strategic decisions to develop new products and retain customers.
- This study focuses on dividing customers into different groups in which data points in a similar group will have similar properties, and also provides insight into what factors should be considered when retaining customers.

The study consists of:<br><br>
<a href='#1.0'>Functions to be used</a><br>
    <blockquote>
        <a>Pandas</a><br>
        <a>Visualization</a><br>
        <a>Encoding</a><br>
        <a>Scaler (Standard, MinMax)</a><br>
    </blockquote>
<a href='#2.0'>Import Libraries</a><br>
<a href='#3.0'>Load Data</a><br>
    <blockquote>
        <a>Overview of all features</a><br>
  <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169572835-7e8a3d60-38ea-43e8-9fae-bf136cca45fa.png"> <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169572972-38ff872e-e44b-4f64-9f39-223ea7fd5712.png">
    </blockquote>
<a href='#4.0'>Exploratory Data Analysis (EDA)</a><br>
    <blockquote>
        <a>Analyze each feature</a><br>
  <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169573198-3058ad18-ba31-4285-85e5-b15ff683354b.png">
<img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169573265-c7aa6f73-fb36-4cfd-a272-90e004200da2.png">
<img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169573332-be6174ee-1be5-4fee-8133-66e6f00cc221.png">
    </blockquote>
<a href='#5.0'>Clustering</a><br>
<blockquote>
    <a>Principal Component Analysis (PCA)</a><br>
  <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169573462-6b13b7fa-7168-4c34-9a7d-e136c9ffa2ee.png">
    <a>KMeans</a><br>
          <blockquote>
            <a>Selecting the number of clusters</a><br>
            <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169573526-b2ca059c-5500-4fb7-9f27-897fb8ab33d7.png"> <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169573621-767395f7-6694-4fa6-a9e0-e605a586f9f5.png"> <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169573684-24b8f5b9-ae32-4648-9e4e-a1c90625143e.png"><br>
            <a>Run KMeans with the optimal number of clusters</a><br>
            <img width="230" alt="image" src="https://user-images.githubusercontent.com/58983814/169573754-cdf82aa3-a1f1-446d-b9bc-7aeac33e137f.png"><br>
            <a>Evaluation Metrics</a><br>
            <a>Visualise Clusters (Standard, MinMax)</a><br>
            <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169574024-6423ff72-0509-40ef-a90e-7e576c3318f7.png"><br>
          </blockquote>
    <a>Hierarchical clustering</a><br>
          <blockquote>
              <a>Dendrogram to find the optimal number of clusters</a><br>
            <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169574109-1af3b077-9db5-4398-9cf1-633f44dcb610.png"><br>
              <a>Run the hierarchical clustering with the optimal number of clusters</a><br>
              <a>Evaluation Metrics</a><br>
              <a>Visualise Clusters</a><br>
          </blockquote>
    <a>DBSCAN</a><br>
          <blockquote>
              <a>Finding best values of eps and min_samples</a><br>
            <img height="100" alt="image" src="https://user-images.githubusercontent.com/58983814/169574232-c4a29dd2-f006-441b-ac30-74496049d105.png"><br>
          </blockquote>
    <a>Add clustering labels to the main dataframe and analyze</a><br>
</blockquote>
