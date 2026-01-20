# assignment-sampling-

Sampling Techniques:
In classification tasks with imbalanced datasets (e.g., 90% majority vs. 10% minority class), models often bias toward the majority class, leading to poor minority class prediction. Sampling techniques adjust class distributions to balance the data, improving model fairness and accuracy without altering the underlying model.

a) Random Under-Sampling (RUS)
Randomly removes instances from the majority class to match the minority class size. This balances the dataset but risks losing valuable information from the majority class, potentially reducing overall model performance. 

b) Random Over-Sampling (ROS)
Randomly duplicates minority class instances to equal the majority class count. It preserves all original data but can lead to overfitting due to repeated samples, making the model less generalizable.

c) SMOTE (Synthetic Minority Oversampling Technique)
Creates synthetic minority samples by interpolating between existing minority instances in feature space. This introduces diverse, realistic data points, balancing the dataset while mitigating overfitting risks compared to simple duplication.

d) NearMiss
An intelligent under-sampling method that selects majority class samples nearest to minority samples based on distance metrics.

e) Tomek Links
Identifies and removes pairs of nearest neighbors from opposite classes that are ambiguous or overlapping. This cleans the dataset by eliminating noise and improving class separability.

Models Used:
a) Logistic Regression (LR)
A linear model that uses the logistic function to predict binary class probabilities based on feature weights.

b) Decision Tree (DT)
Recursively splits data based on feature thresholds to form a tree structure for classification. It handles non-linear relationships and is highly interpretable, allowing easy visualization of decisions.

c) Random Forest (RF)
An ensemble method averaging predictions from multiple decision trees, each trained on a random subset of data. It reduces overfitting, handles high-dimensional and complex data well.

d) Support Vector Machine (SVM)
Finds the optimal hyperplane to maximize the margin between classes in a high-dimensional space.

e) K-Nearest Neighbors (KNN)
Classifies a sample by majority vote of its k closest neighbors in feature space. It's simple, non-parametric, and adapts to any data distribution without assumptions.

