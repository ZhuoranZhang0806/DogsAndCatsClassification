# 🐶🐱 Dogs vs Cats Classification

**Practical Lab 3 — Deep Learning Models for Image Classification**

---

## 📌 Project Overview

This project focuses on binary image classification of **cats and dogs** using deep learning models.

Two pre-trained convolutional neural networks are implemented:

* **VGG16 (Fine-Tuned)**
* **MobileNetV2 (Transfer Learning + Fine-Tuning)**

The objective is to explore how transfer learning improves performance compared to traditional approaches and to analyze model behavior using multiple evaluation metrics.

---

## 🎯 Objectives

* Apply **transfer learning using pre-trained models**
* Perform **fine-tuning to improve model performance**
* Evaluate models using multiple metrics
* Analyze model errors and limitations
* Compare different deep learning architectures

---

## 📂 Dataset

The dataset consists of labeled images of cats and dogs, divided into:

```id="8y3c7n"
data/
│
├── train/
├── validation/
└── test/
```

Each subset contains two categories:

* `cat`
* `dog`

---

## 🧠 Models

### 1️⃣ VGG16 (Fine-Tuned)

VGG16 is a deep convolutional neural network pre-trained on ImageNet.

**Approach:**

* Load pre-trained weights
* Freeze convolutional layers
* Train custom classifier
* Unfreeze top layers for fine-tuning

---

### 2️⃣ MobileNetV2

MobileNetV2 is a lightweight and efficient architecture optimized for speed and performance.

**Advantages:**

* Faster training
* Fewer parameters
* Strong generalization ability

---

## ⚙️ Methodology

1. Load dataset using `image_dataset_from_directory`
2. Apply preprocessing using model-specific normalization
3. Train models using transfer learning
4. Fine-tune selected layers
5. Evaluate models on the test dataset

---

## 📊 Evaluation Metrics

The models are evaluated using:

* Accuracy
* Confusion Matrix
* Precision, Recall, F1-score
* Precision-Recall Curve
* Error Analysis

---

## 📈 Results Summary

| Model       | Accuracy |
| ----------- | -------- |
| VGG16       | ~94%     |
| MobileNetV2 | ~98%     |

---

## 🔍 Key Findings

* Transfer learning significantly improves classification performance
* MobileNetV2 achieves higher accuracy and better generalization
* VGG16 performs well but shows more sensitivity to complex images
* Both models perform consistently across classes

---

## ⚠️ Challenges

* Some images are visually ambiguous
* Lighting conditions and background noise affect predictions
* Misclassifications occur in low-quality or complex images

---

## 💡 Conclusion

This project demonstrates that transfer learning is highly effective for image classification tasks.

MobileNetV2 achieves the best performance due to its efficient architecture, while VGG16 provides stable but slightly lower results.

---

## 🚀 Future Work

* Add baseline model (Vanilla CNN) for comparison
* Apply data augmentation
* Experiment with other architectures (ResNet, EfficientNet)

---

## 🛠️ Requirements

* Python 3.x
* TensorFlow / Keras
* NumPy
* Matplotlib
* scikit-learn

---

## 👤 Author

Zhuoran Zhang 9048508
Conestoga College
Applied AI & Machine Learning

---

## 🔗 Repository

GitHub Repository:  
https://github.com/ZhuoranZhang0806/DogsAndCatsClassification.git
