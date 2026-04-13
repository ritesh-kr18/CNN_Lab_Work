# Deep Learning CNN Lab (CIFAR-10)

This project implements a complete deep learning pipeline for image classification on the CIFAR-10 dataset using **PyTorch**.

---

## 📌 Framework Used
- PyTorch (torch, torchvision)

---

## 📂 Project Overview

This lab covers:

- CNN implementation from scratch  
- Training and regularisation (BatchNorm, Dropout)  
- Learning rate scheduling  
- Feature visualisation (filters & feature maps)  
- Grad-CAM interpretability  
- Confusion matrix & classification report  
- Transfer learning (ResNet18)  
- Fine-tuning and ablation study  
- Benchmark: Scratch vs Transfer Learning  

---

## 📊 Results Summary

| Model | Test Accuracy |
|------|-------------|
| Scratch CNN | 0.749 |
| Transfer (Frozen) | 0.479 |
| Transfer (Fine-tuned) | 0.616 |

---

## 📈 Key Observations

- Scratch CNN performed best due to full adaptation to CIFAR-10  
- Frozen transfer model underperformed due to lack of feature adaptation  
- Fine-tuning improved performance by adapting higher-level features  
- Grad-CAM shows model focuses on important regions for prediction  

---

## 🖼️ Visualisations

Includes:
- Training curves  
- Confusion matrix  
- Grad-CAM heatmaps  
- Feature maps  
- Learned filters  

---

## 📦 Dataset

- CIFAR-10 (automatically downloaded using torchvision)

> Note: The dataset folder is excluded from the repository due to size constraints.

---

## ▶️ How to Run

Install dependencies:

```bash
pip install torch torchvision matplotlib seaborn scikit-learn

jupyter notebook 24cd3035_CNN_Lab.ipynb
