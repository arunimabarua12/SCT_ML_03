# SCT_ML_03
# 🐶🐱Dog vs Cat Image Classification

# 📌 Overview

This project solves the classic dog vs. cat classification problem without deep learning. Instead, it leverages a multi-feature extraction strategy combined with Support Vector Machines (SVM), Random Forest (RF), and an Ensemble Voting Classifier to achieve robust results.

It supports:

Batch prediction for multiple test images.

Single image prediction with confidence score.

Visual performance analysis (Confusion Matrix & Classification Report).

# 📂Download Dataset
- **Data Source**: https://www.kaggle.com/c/dogs-vs-cats/data

Place the Kaggle Dogs vs Cats dataset inside:
/train/train/

Images must be named like dog.123.jpg, cat.456.jpg.

# 📂Test Dataset
The repository supports both sample test images and an optional full test dataset to evaluate model predictions.

- **Dataset** : https://www.kaggle.com/datasets/arunimabarua/test-dog-cat/settings

 
# 🧠 Key Features

✅ Multi-technique feature extraction:
-  HOG (Histogram of Oriented Gradients) 
-  LBP (Local Binary Pattern)    
-  Gabor filters (frequency & orientation analysis)   
-  Color features (RGB, HSV, LAB statistics)

✅ PCA for dimensionality reduction (retains 95% variance)

✅ GridSearchCV hyperparameter tuning for both SVM and RF

✅ Ensemble Learning using soft voting

✅ Confusion matrix & classification reports

✅ Batch prediction and single image inference

🗂️ Project Structure

dog-cat-ml/
├── main_script.py # Main training and prediction script
├── README.md # Project documentation
├── requirements.txt # Dependencies
├── /train/train/ # Training images (Kaggle-style: cat.123.jpg, dog.456.jpg)
├── /test-dog-cat/ # Test images for batch prediction


# ➤ What it does:
Loads and preprocesses images.

Extracts features using HOG, LBP, Gabor, and Color Stats.

Applies scaling + PCA.

Trains optimized SVM and RF using GridSearchCV.

Builds an ensemble classifier.

Evaluates performance and makes predictions on test images.

# Example Output
<img width="781" height="514" alt="image" src="https://github.com/user-attachments/assets/ce1921f4-2079-43e6-b1bc-4d3165157b48" />
<img width="475" height="634" alt="image" src="https://github.com/user-attachments/assets/db102d16-cb33-4676-94ca-55d7e733c6ee" />


# 📊 Performance Evaluation
After training, the model prints:

Accuracy score

Detailed classification report

Confusion matrix (with visualization)

# 🛠 Future Improvements
 Add real-time webcam prediction (OpenCV GUI).

 Export models using joblib or pickle for deployment.

 Build a web app with Streamlit or Flask for interactive use.

 Expand to other animals (multi-class classification).

