# Face Recognition using Principal Component Analysis (PCA)

🌐 **Face Recognition using Principal Component Analysis (PCA)** 🌐

This repository showcases a facial recognition system using PCA, specifically projecting face images onto the "Eigenfaces," which are the eigenvectors of the face dataset. The objective is to recognize faces by comparing them to a pre-existing database.

PCA is employed to generate k eigenfaces (here, I have chosen 50) for a training set of M images (400), thereby reducing the number of values from M to k needed to identify an unknown face.

📄 **Read the Paper on Eigenfaces:** [Eigenfaces Paper](https://sites.cs.ucsb.edu/~mturk/Papers/mturk-CVPR91.pdf)

📂 About the Dataset:
# The ORL Face Database


## Dataset Details:
- 10 different images of 40 distinct subjects.
- Variations include different times, lighting conditions, facial expressions (open/closed eyes, smiling/non-smiling), and facial details (glasses/no-glasses).
- Images taken against a dark homogeneous background, with subjects in an upright, frontal position (with tolerance for some side movement).

## Image Format:
- Files in PGM format.
- Viewable using the 'xv' program.
- Each image is 92x112 pixels with 8-bit grey levels.

## Organization:
- Images are organized in 40 directories (one for each subject) named as: `sX` where X is the subject number (between 1 and 40).
- Each directory contains 10 different images of the selected subject named as: `Y.pgm` where Y indicates the image for the specific subject (between 1 and 10).

**Explore the ORL Face Database:**
[Learn More](https://www.kaggle.com/datasets/kasikrit/att-database-of-faces)





# 🚀 Tasks Performed

This repository details the following tasks performed in the Face Recognition using Principal Component Analysis (PCA) project:

1. **Loading Dataset and Splitting:**
   - Loaded the dataset.
   - Divided the data into training and test sets.One split was 50-50 and other was 70-30 .The results are discussed in n

2. **Implementing PCA Algorithm from Scratch:**
   - Developed the PCA algorithm from scratch.

3. **Implementing Image Reconstruction:**
   - Utilized eigen projections for image reconstruction.
   - Visualized differences for varying numbers of components.

4. **Visualizing Mean (Eigen Face) Generation:**
   - Visualized the mean (Eigen face) generated from the dataset.

5. **Face Recognition Module:**
   - Developed a face recognition module.
   - Obtained accuracy on the training set.
   - Evaluated accuracy for different numbers of training images.
# Principal Component Analysis (PCA) for Face Recognition

Principal Component Analysis (PCA) is a technique for reducing the dimensionality of data by capturing the maximum variance in the dataset. When applied to face recognition, PCA helps in representing facial features in a lower-dimensional space. Here's a step-by-step guide:

## Steps:

1. **Standardize the Dataset:**
   - Subtract the mean and divide by the standard deviation for each feature to ensure zero mean and unit variance, avoiding bias and scale issues in the data.

2. **Calculate Covariance Matrix:**
   - Compute a square matrix that measures how each feature varies with respect to others. Diagonal elements are variances, and off-diagonal elements are covariances.

3. **Eigenvalues and Eigenvectors:**
   - Solve the equation $Cv = \lambda v$ to obtain eigenvalues and eigenvectors. Eigenvalues represent the variance explained by each eigenvector, and eigenvectors represent directions of new variables (principal components) orthogonal to each other.

4. **Sort Eigenvalues and Eigenvectors:**
   - Arrange in descending order based on eigenvalues, storing them in a matrix where each column is an eigenvector, and each row is an eigenvalue.

5. **Pick k Eigenvalues:**
   - Choose k based on the desired level of information preservation or compression. A common criterion is to select k such that the cumulative sum of the k largest eigenvalues is at least a certain percentage (e.g., 95%) of the total sum of all eigenvalues. The matrix of eigenvectors, also called the feature vector, is formed by taking the first k columns of the sorted matrix.

6. **Transform the Original Matrix:**
   - Multiply the standardized data matrix by the feature vector matrix to generate a new matrix of lower dimensionality. Each row represents a new observation, and each column is a principal component. This matrix can be used for face recognition by comparing distances or similarities between rows, representing faces in terms of principal components.
# Results and Discussion 
## Table 1. Correct recognition rate  with variable number of training samples 
| Training Samples | Testing Samples | CRR (%)  |
|-------------------|------------------|-------|
| 5                 | 5                | 78    |
| 6                 | 4                | 90    |
| 7                 | 3                | 91    |
| 8                 | 2                | 93.75 |
| 9                 | 1                | 95    |
## Conclusion As the number of training samples increases from 5 to 9, the Correct Recognition Rate (CRR) also increases. This suggests that having more diverse training samples positively influences the recognition accuracy.

