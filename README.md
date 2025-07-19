📌 Purpose of the Lab
The primary objective of this lab is to explore and compare two supervised classification algorithms—K-Nearest Neighbors (KNN) and Radius Neighbors (RNN)—using the Wine dataset from the sklearn library. By experimenting with different values of k and radius, this lab aims to highlight how hyperparameter tuning affects classification accuracy and model performance.

🔍 Key Insights & Observations
KNN Performance:
The accuracy of the KNN classifier was found to vary significantly with different values of k. A moderate value (e.g., k=5 or k=11) offered the highest classification accuracy, avoiding both overfitting (low k) and underfitting (high k).

RNN Performance:
The RNN classifier was more sensitive to the choice of radius. Certain radius values (e.g., r=450) produced better accuracy, while larger radii (e.g., r=600) led to reduced performance due to classification ambiguity.

Model Comparison:
KNN showed more stable and consistent performance across different values compared to RNN. However, RNN may be preferable when feature scales are normalized and the data has clear cluster boundaries.

Visualization:
Line plots comparing accuracy trends helped to visually determine optimal parameter ranges for both algorithms.

⚠️ Challenges Faced & Decisions Made
Data Scaling:
Radius Neighbors requires normalized data. This was addressed by using StandardScaler to preprocess features before applying the RNN model.

Model Tuning:
Selecting the right range of k and radius was crucial. Initially, the range was too narrow, and expanding it helped reveal more performance variations.

Overfitting Risk:
For low k values in KNN (e.g., k=1), the model performed well on training but poorly on testing, indicating overfitting. This led to emphasizing moderate k values in evaluation.

Visualization Clarity:
Labels, titles, and markers were added to plots to clearly indicate the performance trends and make insights more interpretable.
