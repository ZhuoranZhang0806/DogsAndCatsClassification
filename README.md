
Each subset contains two categories:

* `cat`
* `dog`

---


## 🧠 Models

### 1️⃣ Vanilla CNN (Baseline)

A simple CNN built from scratch.

**Purpose:**

* Establish baseline performance
* Understand limitations of training without pre-trained features

**Limitations:**

* Lower accuracy
* Prone to overfitting
* Weak feature extraction ability

---

### 2️⃣ VGG16 (Fine-Tuned)

VGG16 is a deep convolutional neural network pre-trained on ImageNet.

**Approach:**

* Load pre-trained weights
* Freeze convolutional base
* Train custom classifier
* Unfreeze top layers for fine-tuning

**Characteristics:**

* High accuracy
* Strong feature extraction
* Computationally expensive

---

### 3️⃣ MobileNetV2

MobileNetV2 is a lightweight architecture optimized for efficiency.

**Advantages:**

* Faster training
* Fewer parameters
* Strong generalization ability

---

## 🤔 Why Three Models?

Although the original requirement only asked for **two models**, this project includes **three models** to provide a more comprehensive comparison and deeper analysis.

The motivation for selecting these three models is:

* **Vanilla CNN (Baseline Model)**  
  Used to establish a reference point. It shows how a model performs when trained from scratch without pre-trained knowledge.

* **VGG16 (Deep Pre-trained Model)**  
  Represents a **high-capacity, deep architecture** with strong feature extraction ability. It helps evaluate the impact of model depth and complexity.

* **MobileNetV2 (Lightweight Pre-trained Model)**  
  Represents an **efficient and optimized architecture**, designed for speed and lower computational cost while maintaining high performance.

---

### 🎯 Key Idea

By selecting these three models, the project enables a meaningful comparison across:

* Baseline vs Transfer Learning
* Heavy vs Lightweight architectures

---

## ⚙️ Methodology

1. Load dataset using `image_dataset_from_directory`
2. Apply preprocessing and normalization
3. Train baseline CNN model
4. Apply transfer learning (VGG16, MobileNetV2)
5. Fine-tune selected layers
6. Evaluate models on test dataset

---

## 📊 Evaluation Metrics

The models are evaluated using:

* Accuracy
* Confusion Matrix
* Precision, Recall, F1-score
* Precision-Recall Curve
* Training History (Loss & Accuracy)
* Error Analysis

---

## 📈 Results Summary

| Model        | Accuracy |
|-------------|--------|
| Vanilla CNN | ~50%   |
| VGG16       | ~94%   |
| MobileNetV2 | ~98%   |

---

## 🔍 Key Findings

* Transfer learning significantly improves performance over baseline CNN
* Vanilla CNN performs close to random guessing due to limited feature learning
* MobileNetV2 achieves the best performance with high efficiency
* VGG16 provides strong but computationally heavier results
* Pre-trained models generalize better on unseen data

---

## 🧠 Thinking Points

### 🔹 Vanilla CNN
* Performs poorly due to lack of pre-trained features
* High risk of overfitting
* Weak generalization ability

### 🔹 MobileNetV2
* Efficient and lightweight
* Strong balance between speed and accuracy
* Best overall performance

### 🔹 VGG16
* Deep architecture enables strong feature extraction
* Higher computational cost
* Stable but slightly less efficient than MobileNetV2

---

## ⚠️ Challenges

* Some images are visually ambiguous
* Lighting conditions and background noise affect predictions
* Misclassification occurs in complex or low-quality images
* Class boundaries are sometimes unclear

---

## 💡 Conclusion

This project demonstrates that **transfer learning is highly effective** for image classification tasks.

* **MobileNetV2** achieves the best performance due to efficiency and generalization  
* **VGG16** provides strong and stable results but is computationally heavier  
* **Vanilla CNN** highlights the importance of pre-trained feature extraction  

---

## 🚀 Future Work

* Apply advanced data augmentation
* Experiment with other architectures (ResNet, EfficientNet)
* Hyperparameter tuning
* Use larger and more diverse datasets

---

## 🛠️ Requirements

* Python 3.x
* TensorFlow / Keras
* NumPy
* Matplotlib
* scikit-learn

---

## 👤 Author

Zhuoran Zhang — 9048508  
Conestoga College  
Applied AI & Machine Learning

---

## 🔗 Repository

GitHub Repository:  
https://github.com/ZhuoranZhang0806/DogsAndCatsClassification.git