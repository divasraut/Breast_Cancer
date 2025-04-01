# Breast_Cancer
Breast Cancer -This project focuses on classifying breast cancer tumors as malignant or benign using Principal Component Analysis (PCA) and Support Vector Machine (SVM).
The final model is evaluated using accuracy and classification reports, and the PCA-transformed data is visualized for better interpretability. This approach ensures efficient, accurate, and robust tumor classification, helping in early diagnosis and decision-making. 🚀

Step 1: Import Required Libraries
Purpose:
pandas and numpy → Used for handling datasets and arrays.
load_breast_cancer → Loads the Breast Cancer dataset from sklearn.
matplotlib.pyplot → Used for visualization.

Step 2: Load the Breast Cancer Dataset
Purpose:Loads the dataset into memory.

Step 3: Checking Dataset Structure
Purpose:
Lists available attributes inside the dataset, including:
data → Features
target → Labels
feature_names → Column names

Step 4: Convert Dataset into a DataFrame
Purpose:
Converts the dataset into a structured Pandas DataFrame.

Step 5: Add the Target Column
Purpose:
Adds the target labels (0 = Malignant, 1 = Benign) to the dataset.

Step 6: Display the First Few Rows
Purpose:
Shows the first 5 rows of the dataset for inspection.

Step 7: Check Dataset Shape
Purpose:
Displays the dataset’s dimensions (rows, columns).

Step 8: Standardizing the Data

Why Standardization?
PCA is scale-sensitive.
Standardization ensures each feature has zero mean and unit variance, preventing bias due to different feature magnitudes.

Step 9: Importing PCA
Purpose:
Imports the Principal Component Analysis module.

Step 10: Applying PCA (Reducing to 2 Components)
Why?
Reduces dataset dimensions to 2 principal components for easier visualization and faster model training.

Step 11: Transform Data Using PCA
Purpose:
Applies PCA transformation to reduce features while preserving important information.

Step 12: Train-Test Split
Why?
Splits data into 70% training and 30% testing for fair model evaluation.
random_state=1 ensures consistent results across multiple runs.

Step 13: Training an SVM Model
Why SVM?
SVM is effective for high-dimensional data.
Linear kernel is used since PCA reduces dimensions to a simpler linear space.

Step 14: Evaluating Model Performance
Predicts labels for test data.
Prints Precision, Recall, and F1-score for performance analysis.

Step 15: PCA Visualization
Purpose:
Creates a 2D scatter plot of PCA-transformed data, colored by class labels.

Summary of Steps
Loaded the Breast Cancer dataset.

Converted it into a Pandas DataFrame.

Added target labels.

Checked dataset structure and shape.

Standardized features to improve PCA performance.

Applied PCA to reduce dimensions from 30 to 2.

Split the dataset into training and testing sets.

Trained an SVM model with a linear kernel.

Predicted and evaluated model performance.

Visualized PCA-transformed data.

