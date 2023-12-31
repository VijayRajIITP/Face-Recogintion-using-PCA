# Face-Recogintion-using-PCA
🌐 Face Recognition using Principal Component Analysis (PCA) 🌐

This repository showcases a facial recognition system using PCA, specifically projecting face images onto the "Eigenfaces," which are the eigenvectors of the face dataset. The objective is to recognize faces by comparing them to a pre-existing database.

📄 Read the Paper on Eigenfaces

📂 About the Dataset:
The AT&T face dataset features grayscale images of dimensions 92x112. The dataset is organized into 40 subject directories, each containing ten images with various facial expressions, lighting conditions, and details. Explore the AT&T Face Dataset

🚀 Tasks Performed:

Dataset Handling: Loaded and divided data into training and test sets.
PCA Algorithm: Implemented PCA from scratch.
Image Reconstruction: Implemented image reconstruction using eigen projections and visualized differences for different component counts.
Visualization: Explored visualizations, including mean (Eigen face) generation.
Face Recognition Module: Achieved accuracy on the training set for different principal components.
🔧 Steps for PCA Implementation:

Standardize the Data: Ensure zero mean and unit variance.
Compute Covariance Matrix: Reveal feature relationships.
Compute Eigenvectors and Eigenvalues: Identify principal components.
Select Principal Components: Form a new lower-dimensional space.
💡 Advantages of PCA:

Reduces variables, simplifying analysis.
Increases interpretability and visualization.
🛑 Limitations of PCA:

Assumes linear relationships.
Sensitivity to outliers.
Requires data scaling.
In the context of Face Recognition:

Limited ability to capture all facial variations.
Accuracy may be insufficient for high-security applications.
Computational challenges with large datasets.
Explore the power of PCA in facial recognition! 🤖✨ #FacialRecognition #PCA #Eigenfaces #DataScience

Feel free to contribute and enhance the capabilities of this face recognition system! 🚀






