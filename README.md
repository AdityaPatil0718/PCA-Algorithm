# PCA-Algorithm

**Aim:**

Implement Principal component analysis for dimensionality reduction of datapoints.

**Theory:**

Principal Component Analysis (PCA) is a dimensionality reduction technique widely used in data analysis and machine learning. Its primary goal is to transform high-dimensional data into a lower-dimensional representation, capturing the most important information.
How does PCA works:
1. Standardization
   Standardize the data when features are measured in diverse units. This entails subtracting the mean and dividing by the standard deviation for each feature. Failure to standardize data with features of             varying scales can result in misleading components.
2. Compute the Covariance Matrix
   Calculate the covariance matrix as discussed earlier
3. Calculate Eigenvectors and Eigenvalues
   Determine the eigenvectors and eigenvalues of the covariance matrix.

 ![image](https://github.com/AdityaPatil0718/PCA-Algorithm/assets/128233555/5e31480a-b080-4a7e-9a02-0817eee7aff1)

Eigenvectors represent the directions (principal components), and eigenvalues represent the magnitude of variance in those directions. To understand what eigenvectors and eigenvalues are, you can go through this video:
4. Sort Eigenvalues
  Sort the eigenvalues in descending order. The eigenvectors corresponding to the highest eigenvalues are the principal components that capture the most variance in the data. 
5. Select Principal Components
  Choose the top k eigenvectors (principal components) based on the explained variance needed. Typically, you aim to retain a significant portion of the total variance, like 85%. 
6. Transform the Data
  Now, we can transform the original data using the eigenvectors:
So, if we have m dimensional original n data points then 
X : m*n
P : k*m
Y = PX : (k*m)(m*n) = (k*n)
Hence, our new transformed matrix has n data points having k dimensions.


**Conclusion:**
  
PCA is a powerful technique for dimensionality reduction that can significantly reduce the number of features while preserving most of the variability in the data.
