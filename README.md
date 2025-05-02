 <h1>IMDb_ML_Alg </h1>
  <ul>
  Welcome! This project explores predicting whether a movie will be highly rated using a machine learning model trained on IMDb data. The goal: identify the most effective algorithm for the task.</h2>
  </ul>
<h2> Project Overview</h2>
  <ul>
    <li>Dataset: IMDb non-commercial datasets (joined via tconst) - https://datasets.imdbws.com/</li>
    <li>Objective: Predict if a movie receives an average rating of 7.0 or higher (binary classification) </li>
    <li>Key Challenge: Selecting and tuning models for best accuracy while managing class imbalance</li>
  </ul>
<h2>Dataset Details</h2>
<ul>

  <li>100,000 movies included</li>
  <li>Two versions: one including adult content, one excluding it</li>
  <li> Preprocessing included Mean replacement for missing runtimeMinutes, One-hot encoding for multi-genre support, Feature scaling (where appropriate), and Binary target based on average rating (≥ 7.0 → "Highly Rated")</li>
</ul>
<h2>ML Models Used</h2>
<ul>
  <li>Logistic Regression: Best for linear, binary classification tasks</li>
  <li>K-Nearest Neighbors (KNN): Useful for similarity-based, non-parametric classification</li>
  <li>Naïve Bayes: Fast and effective for independent categorical feature</li>
  <li>Decision Trees: Handles non-linear patterns with mixed data types</li>
  <li>Neural Networks (TensorFlow): Captures complex, non-linear relationships</li>
</ul>
<h2>Results</h2>
  <ul>
    <li>Logistic Regression	is best for Simple, interpretable, decent for linearly separable data</li>
    <li>KNN	Struggled with this project as it gets worse with higher dimensions and noisy features</li>
    <li>Decision Tree	was good with our mixed data, but was prone to overfitting</li>
    <li>Naïve Bayes was fast but assumes feature independence</li>
    <li>Neural Network was the most complex model, only marginal gains due to data limits, but highest overall accuracy</li>
  </ul>
