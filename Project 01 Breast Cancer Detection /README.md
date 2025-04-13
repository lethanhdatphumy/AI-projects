# 🧠 Project 1 – Breast Cancer Detection with CNN

This project uses deep learning to classify breast cancer histopathology images from the [BreakHis dataset](https://www.kaggle.com/datasets/ambarish/breakhis). It’s part of my personal journey to learn applied AI through hands-on, research-inspired projects.

---

## 📌 Project Goals

- Understand and replicate key ideas from the paper:  
  _“Breast Cancer Histopathological Image Classification using Deep Neural Networks” (Spanhol et al.)_
- Build a preprocessing pipeline to extract crops and apply stain-style color augmentation
- Train a CNN to classify cancerous tissue
- (Upcoming) Add Grad-CAM for interpretability

---

## 🧪 Dataset

- **BreakHis dataset** – histopathology images of benign and malignant tumors
- Each image is taken at different magnifications (e.g., 40X, 100X, 200X, 400X)

---

## 🧰 Techniques Used

- **Random crop extraction** (20 crops per image)
- **Color augmentation** (50 brightness-scaled variations per crop)
- **Preprocessing**: Resize to 224×224, normalize pixel values
- (Next steps) **CNN feature extractor + 3-norm pooling**

---

## 🔄 Current Pipeline Output

- For each image:
  - Extract 20 random crops
  - Generate 50 augmentations per crop
  - Final shape: `(20, 50, 224, 224, 3)`

---

## ✅ What I’ve Learned

- How to preprocess medical images using random crops and augmentation
- The importance of stain variation in histology
- How to structure a clean image pipeline in Python
- When and why to use RGB conversion and clipping

---

## 🧠 Next Steps

- Build and train CNN on processed data
- Add Grad-CAM visualizations
- Apply 3-norm pooling to combine crop features into a single descriptor
- Train a final classifier (e.g., Gradient Boosting or Dense)

---

## 💻 Repo Structure
