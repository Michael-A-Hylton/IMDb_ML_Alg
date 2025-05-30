 <h1>IMDb_ML_Alg: Predicting Highly Rated Movies Using Machine Learning</h1>
  <ul>
  Welcome! This project explores predicting whether a movie will be highly rated using a machine learning model trained on IMDb data. The goal: identify the most effective algorithm for the task.</h2>
  </ul>
<h2> Project Overview</h2>
  <ul>
    This project investigates the use of machine learning algorithms to predict whether a movie is likely to be highly rated. The central objective is to determine the most effective classification algorithm for this task using publicly available IMDb datasets.
    The primary objective was to predict whether a movie receives an average IMDb rating of 7.0 or higher (binary classification: "Highly Rated" vs. "Not Highly Rated"). I wanted to achieve a high classification accuracy while addressing class imbalance and selecting appropriate models.
  </ul>
<h2>Dataset Details</h2>
<ul>
  The project utilizes non-commercial IMDb datasets available at IMDb Datasets. Multiple files were joined using the tconst identifier to compile a comprehensive dataset.
  The dataset used contained pproximately 100,000 movies entries. Two different datasets were prepared—one including movies with adult content and one excluding it to see how additional information would aid training. The dataset was preprocessed using mean replacement for missing values, one-hot encoding to support multi-genre training, scaling on numeric features, and created a binary target based on average rating (≥ 7.0 → "Highly Rated" -> 1)
</ul>
<h2>ML Models Used</h2>
The following machine learning algorithms were evaluated:
<ul>
 
  <li>Logistic Regression: A linear model suitable for binary classification. Provides a good baseline and interpretable output.</li>
  <li>K-Nearest Neighbors (KNN): A non-parametric model based on feature similarity. Sensitive to feature scaling and high dimensionality.</li>
  <li>Naïve Bayes: A probabilistic model well-suited for categorical data under the assumption of feature independence.</li>
  <li>Decision Trees: A flexible model that handles both categorical and numerical data. Captures non-linear relationships but can overfit.</li>
  <li></li>Neural Networks (TensorFlow): Designed to learn complex patterns in data. Offers strong performance on non-linear problems with sufficient data.</li>
</ul>
<h2>Results</h2>
  Each model's performance was assessed with respect to accuracy, interpretability, and robustness:
  <ul>
    <li>Each model's performance was assessed with respect to accuracy, interpretability, and robustness:</li>
    <li>Logistic Regression: Delivered solid performance for linearly separable data. Interpretable and easy to tune.</li>
    <li>K-Nearest Neighbors: Underperformed due to high dimensionality and noisy features, which impacted similarity calculations.</li>
    <li>Decision Tree: Handled mixed data types well but exhibited overfitting, especially on the training set.</li>
    <li>Naïve Bayes: Fast and efficient, but performance was limited by the assumption of feature independence.</li>
   <li>Neural Network: Achieved the highest overall accuracy. However, performance gains were only marginal due to data limitations and model complexity.</li>
  </ul>
