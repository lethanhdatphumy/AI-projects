# 🧠 Breast Cancer Detection from Histopathology Images (BreakHis + CNN)

This project applies Convolutional Neural Networks (CNNs) to detect breast cancer from histopathology images using the [BreakHis dataset](https://www.kaggle.com/datasets/ambarish/breakhis). It’s inspired by the research paper:

> Spanhol et al., “Breast Cancer Histopathological Image Classification using Deep Neural Networks” (2016)

---

## 📌 Project Objectives

- Reproduce key parts of the paper in a project-based learning format
- Explore preprocessing techniques for medical images:
  - Random crop extraction
  - Color augmentations simulating stain variations
- Train a CNN to classify tissue as benign or malignant
- (In Progress) Add feature pooling and visualization

---

## 🗃️ Dataset

- **BreakHis** – breast histopathology images from 82 patients
- Each image has magnification levels (40X, 100X, 200X, 400X)
- Classification labels: **Benign** vs **Malignant**

📦 Dataset link: [Kaggle – BreakHis](https://www.kaggle.com/datasets/ambarish/breakhis)

---

## 🧪 Techniques Used

- **OpenCV** for image manipulation
- **Random cropping** (20 patches per image)
- **Color augmentation** (50 brightness shifts per crop)
- **CNN modeling** (coming up)
- **3-norm pooling** for multi-crop descriptor fusion (planned)
- **Grad-CAM** visualization (planned)

---

## 🚀 What I’ve Learned So Far

- How to simulate stain variation using brightness augmentation
- How to prepare high-resolution medical images for CNN input
- Why consistent preprocessing (resize, normalize, clip) matters
- How multi-crop input can boost learning from large histology slides

---

## 🔁 Current Pipeline Output

From a single image:
- 20 random crops → each resized to (224, 224)
- 50 color augmentations per crop
- Final shape: `(20, 50, 224, 224, 3)`

---

## 🔧 Repo Structure
