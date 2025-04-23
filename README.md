# 📊 Waste Material Classification and Carbon Footprint Estimation Project

📧 Contact: ogun.atalay33@gmail.com

## 🎯 Project Objective
This project aims to classify waste materials using image data and analyze the environmental impact (carbon footprint) of these materials. The implementation involves both machine learning techniques (Random Forest, Decision Tree, SVM) and deep learning models (MobileNet and custom CNN layers).

## 📁 Dataset Structure and Preparation
- **Data Source:** Kaggle (split-garbage-dataset)
- **Folder Structure:**
  - `Train`: Used for training the model
  - `Test`: Used for evaluating model performance
- **Categories:**
  - Plastic
  - Metal
  - Paper
  - Cardboard
  - Glass
  - Trash
- **Image Preprocessing:**
  - Resized to `224x224` and normalized
  - Applied data augmentation: rotation, shifting, zooming

## 🧠 Deep Learning Models
### MobileNet (Transfer Learning)
- **Base Model:** Pre-trained MobileNet (ImageNet weights)
- **Architecture:**
  - Base layers frozen
  - Custom CNN layers added
  - Final softmax layer based on class count
- **Training:**
  - Trained on training set, validated on validation set
- **Performance:**
  - **Test Accuracy:** 78%
  - Training accuracy and loss were monitored

## 🤖 Machine Learning Models
Features extracted from MobileNet were used with traditional ML classifiers:

### a. Random Forest
- **Goal:** Classify using extracted features
- **Metrics:** Accuracy, Precision, Recall, F1 Score

### b. Decision Tree
- **Goal:** Tree-based classification
- **Metrics:** Accuracy, Precision, Recall, F1 Score

### c. Support Vector Machine (SVM)
- **Goal:** Optimal decision boundary in feature space
- **Metrics:** Accuracy, Precision, Recall, F1 Score

**Best performing model:** Random Forest

## 📊 Visualizations
- **Training Metrics:** Accuracy and loss graphs
- **Carbon Footprint Analysis:**
  - Plastic = highest carbon footprint
  - Trash = lowest carbon footprint
- **Scatter Plot:** Material types vs carbon contributions

## 📸 Example Prediction
- Sample images were tested
- E.g., a plastic waste image was correctly classified

## 🌍 Application Areas
- Smart Waste Management Systems
- Environmental Protection and Recycling Projects
- Industrial Waste Sorting Facilities

## 📝 Conclusion
- Transfer learning (MobileNet) and ML models used effectively
- Random Forest achieved best performance among classical models
- Offers a practical solution for real-world recycling and waste classification
