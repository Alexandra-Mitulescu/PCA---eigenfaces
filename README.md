# Principal Component Analysis (PCA)

## Introduction

This README provides an overview of Principal Component Analysis (PCA), a widely used dimensionality reduction technique in machine learning and data analysis.
PCA aims to transform high-dimensional data into a lower-dimensional space while preserving the most important information or patterns present in the original data.

## Key Concepts

1. **Dimensionality Reduction**: reduces the number of features (dimensions) in a dataset while retaining as much information as possible.
   It is particularly useful when dealing with high-dimensional datasets that may suffer from the curse of dimensionality.

3. **Orthogonal Transformation**: performs an orthogonal linear transformation on the data, which means that the transformed features (principal components) are uncorrelated with each other.
   This property allows for capturing the maximum variance in the data using a smaller number of principal components.

5. **Variance Preservation**: identifies the directions (principal components) along which the data exhibits the highest variance.
   By selecting the top-k principal components, we can preserve a significant amount of the variance in the original data, even with a reduced number of dimensions.

7. **Eigenvalues and Eigenvectors**: PCA calculates the eigenvalues and eigenvectors of the covariance matrix or the correlation matrix of the data.
   The eigenvalues represent the amount of variance explained by each principal component, while the eigenvectors determine the direction of the principal components.

9. **Explained Variance Ratio**: The explained variance ratio indicates the proportion of the total variance in the data explained by each principal component.
    Helps in assessing how much information is retained when reducing the dimensionality.

## Limitations of PCA

- **Loss of Interpretability**: In the transformed space, the principal components may not have a direct interpretation in terms of the original features, making it challenging to explain the meaning of each component.

- **Nonlinear Relationships**: PCA assumes linear relationships between features, which may not capture complex nonlinear dependencies in the data.
   In such cases, nonlinear dimensionality reduction techniques like t-SNE or autoencoders might be more appropriate.

- **Outliers**: PCA is sensitive to outliers as they can strongly influence the calculation of covariance or correlation matrix.
