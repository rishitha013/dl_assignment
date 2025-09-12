# dl_assignment
# 🖼️ Image Classification using ML, CNN, VGG16, and ResNet50  

## Overview  
This project focuses on **image classification** by comparing different approaches:  

- **Traditional Machine Learning (ML)** using handcrafted features (LBP, HOG)  
- **Custom Convolutional Neural Network (CNN)** trained end-to-end  
- **VGG16** (Transfer Learning)  
- **ResNet50** (Transfer Learning, best performance with 90%+ accuracy)  

The goal is to analyze how feature engineering, deep learning, and transfer learning differ in terms of performance and accuracy.  

---

##  Requirements  

Install the required libraries:  

```bash
pip install numpy pandas matplotlib seaborn scikit-learn opencv-python tensorflow keras pillow

---

##  📂 Project Workflow
1. Dataset Preparation

Images organized into folders by class.

Preprocessed: resized (64x64 for ML/CNN, 224x224 for VGG16 & ResNet50).

Converted to grayscale (for ML feature extraction).

2. Feature Extraction (ML)

LBP (Local Binary Patterns)

HOG (Histogram of Oriented Gradients)

Features used with classifiers: Logistic Regression, KNN, Decision Tree, Random Forest, SVM.

3. CNN (Custom Model)

A CNN was built using Keras.

Architecture: Conv → Pooling → Dense → Softmax.

Achieved ~65% accuracy.

4. VGG16 (Transfer Learning)

Pretrained VGG16 model used to extract deep features.

Trained classifiers on these features.

Improved results (~75–80% accuracy).

5. ResNet50 (Transfer Learning)

Pretrained ResNet50 model with fine-tuning.

Input size: 224x224.

Outperformed all methods with 90%+ accuracy.

---

## Conclusion

ML (LBP/HOG): Simple and interpretable, but accuracy is limited.

CNN: Improves results by automatically learning features.

VGG16: Transfer learning adds strong feature representation.

ResNet50: Achieved 90%+ accuracy, proving deep pretrained models are the best choice for image classification in this project.


