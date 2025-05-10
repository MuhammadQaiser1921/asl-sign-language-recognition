# 🤟 ASL Sign Language Recognition using Transfer Learning (MobileNetV2)

This project implements an efficient American Sign Language (ASL) hand sign recognition system using **Transfer Learning** with the **MobileNetV2** architecture. It classifies 29 static ASL signs (A–Z, "space", "nothing", "del") from image data.

## 🧠 Model Details
- **Architecture**: Transfer learning with **MobileNetV2**
- **Input Size**: 128x128x3 RGB images
- **Frozen Base**: `include_top=False`, `weights='imagenet'`
- **Top Layers**:
  - Global Average Pooling
  - Dense Layer with 128 ReLU units
  - Dropout (0.5)
  - Output: Softmax layer for 29 classes
- **Loss Function**: `categorical_crossentropy`
- **Optimizer**: `adam`
- **Metrics**: Accuracy

## 🗃 Dataset
- **ASL Alphabet Dataset** ([Kaggle](https://www.kaggle.com/datasets/grassknoted/asl-alphabet))
- Training Folder: `asl_alphabet_train/`
- Test Folder: `asl_alphabet_test/`
- Classes: `A-Z`, `space`, `nothing`, `del`

## ⚙️ Features
- Transfer learning for faster convergence and higher accuracy
- Lightweight architecture suitable for real-time predictions
- Evaluation using confusion matrix and classification report
- Single image prediction support


![image](https://github.com/user-attachments/assets/3619953d-eed0-409c-b2b8-0560c5e6bb98)
