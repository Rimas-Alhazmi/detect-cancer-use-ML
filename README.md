
This project applies machine learning techniques to classify skin lesions as either **benign or malignant**, using the **ISIC 2024 skin cancer dataset**. The project implements two different models: a **custom-built CNN** and a **transfer learning model using VGG-16**.

## 📂 Dataset
- Source: [ISIC 2024 Challenge on Kaggle](https://www.kaggle.com/competitions/isic-2024-challenge/data)
- Preprocessing: Resized, normalized, and augmented using rotation, zoom, and flipping.
- Split: 
  - 80% Training
  - 20% Validation
  - Test set used for final evaluation

## 🧠 Models Used

### 1. Custom CNN
- Built from scratch
- 3 convolutional layers + max-pooling
- Fully connected + Dropout + Softmax output
- Optimizer: Adam, Loss: Categorical Crossentropy
- Achieved **80.21% Test Accuracy**

### 2. VGG-16 (Transfer Learning)
- Pretrained on ImageNet
- Used as feature extractor with custom classification head
- Output: Sigmoid or Softmax
- Optimizer: Adam, Loss: Binary Crossentropy
- Achieved **53.13% Test Accuracy** (overfitting noted)

## 📊 Results
| Model    | Test Accuracy | Notes              |
|----------|---------------|--------------------|
| CNN      | 80.21%        | Simpler, better generalization |
| VGG-16   | 53.13%        | Overfitted, needs tuning       |

## 🔧 Future Work
- Test deeper models like ResNet, EfficientNet
- More data augmentation to reduce overfitting
- Use ensemble techniques
- Address class imbalance (more malignant samples)

## 👩‍💻 Team
- Remas Alhazmi
- Lama Ahmad
- Maram Haroon
- Roaa Abdulrahman

Instructor: Dr. Asmaa Boughoula  
Department of Artificial Intelligence  
University of Prince Mugrin

---

> 🚀 This project showcases how deep learning can support early skin cancer detection, helping improve healthcare outcomes through automated diagnostics." > README.md
