# Face-Recogintion-using-PCA
🌐 Face Recognition using Principal Component Analysis (PCA) 🌐

This repository showcases a facial recognition system using PCA, specifically projecting face images onto the "Eigenfaces," which are the eigenvectors of the face dataset. The objective is to recognize faces by comparing them to a pre-existing database.
PCA is employed to generate k eigenfaces (here, I have chosen 50) for a training set of M images (400), thereby reducing the number of values from M to k needed to identify an unknown face.
📄 Read the Paper on Eigenfaces(https://sites.cs.ucsb.edu/~mturk/Papers/mturk-CVPR91.pdf)

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
[Learn More](https://www.kaggle.com/datasets/kasikrit/att-database-of-faces****)

Feel free to explore and utilize this dataset for your research and projects! 🚀 #FacialRecognition #Dataset #ORLFaceDatabase #DataScience


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






