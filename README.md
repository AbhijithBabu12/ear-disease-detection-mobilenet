# 👂Ear Disease Detection using MobileNetV2 + Grad-CAM

A deep learning project that classifies different ear diseases from otoscopic images using **MobileNetV2**, optimized for deployment on low-resource hardware (T4 GPU / mobile devices). The model also includes **Grad-CAM visualization** to explain predictions and highlight infected regions.

---

## 🚀 Features

- ✔️ Multi-class classification of ear diseases  
- ✔️ Lightweight MobileNetV2 backbone (fast + small + accurate)  
- ✔️ Grad-CAM heatmaps for visual explanation  
- ✔️ Achieved **high accuracy** on both training & validation sets  
- ✔️ GPU-optimized (Google Colab T4-friendly)  
- ✔️ Clean, modular, reproducible code  

---

## 🧠 Model Architecture

- **Base Model:** MobileNetV2 (ImageNet weights)
- **Input Size:** 224×224  
- **Classifier Head:** GlobalAveragePooling → Dense Layers → Softmax  
- **Loss:** Categorical Crossentropy  
- **Optimizer:** Adam  
- **Regularization:** Dropout  
- **Explainability:** Grad-CAM  

---

## 📊 Results

- **Training Accuracy:** ~99%  
- **Validation Accuracy:** ~99%  
- **Generalization:** No overfitting (curves stable and close)  
- **Grad-CAM:** Correctly highlights infected or inflamed regions  

(Add your plots here if uploading to GitHub)

---

## 📁 Project Structure

├── ear_project.ipynb  # Training notebook

├── otitis_mobilenet_v2.h5

├── otitis_model.tflite

└── otitis_model_quant.tflite

└── otitis_model_quant.tflite

└── README.md

---

---

## 🔥 Grad-CAM Heatmaps

(You can insert sample heatmap images here in GitHub)

---

## 🛠️ Installation

```bash
pip install -r requirements.txt
```
 
## 📦 Exporting the Model

You can export your trained model as:
```bash
model.save("ear_disease_mobilenet.h5")
```
