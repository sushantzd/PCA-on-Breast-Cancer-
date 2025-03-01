# PCA-on-Breast-Cancer-
Principal Component Analysis (PCA) on Breast Cancer Dataset

Overview

This project demonstrates Principal Component Analysis (PCA) on the Breast Cancer dataset from sklearn.datasets. PCA is used for dimensionality reduction while retaining the most important variance in the dataset.

Dataset

The dataset is the Breast Cancer Wisconsin dataset provided by sklearn.datasets.load_breast_cancer().

It contains 30 features representing characteristics of cell nuclei.

The target variable indicates malignant (1) or benign (0) tumors.

Steps Performed

Loaded the dataset using sklearn.datasets.load_breast_cancer().

Standardized the features using StandardScaler to ensure all features have the same scale.

Applied PCA to reduce dimensions while retaining maximum variance.

Visualized the top 2 principal components using a scatter plot with colors representing tumor types.

Plot of 2 Principal Components

To visualize the impact of PCA, a scatter plot of the first two principal components was created:

import matplotlib.pyplot as plt
plt.figure(figsize=(8, 6))
plt.scatter(pca_data[:, 0], pca_data[:, 1], c=cancer.target, cmap='plasma')
plt.xlabel('1st Principal Component')
plt.ylabel('2nd Principal Component')
plt.title('PCA Visualization of Breast Cancer Dataset')
plt.colorbar()
plt.show()

Results

PCA successfully reduced 30 features to 2 principal components.

The scatter plot visually separates malignant and benign tumors based on transformed features.

This confirms that PCA captures important variance, making it useful for dimensionality reduction.

How to Run

Clone the repository and run the script:

git clone <repo_link>
cd <repo_folder>
python pca_breast_cancer.py

Dependencies

Python 3.x

scikit-learn

NumPy

Matplotlib

Pandas

License

This project is open-source and free to use under the MIT License.

