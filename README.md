# Distracted Driver Detection using Deep Learning

## Overview
Driver distraction is one of the major causes of road accidents. This project builds a Deep Learning model to classify driver behavior into multiple categories using image data.

The goal is to automatically detect unsafe activities like texting, talking on the phone, or eating while driving.

---

## Dataset
- Source: https://www.kaggle.com/competitions/state-farm-distracted-driver-detection/data  
- Total Images: 22,000+  
- Classes: 10 categories  

### Classes
- c0 — Safe Driving  
- c1 — Texting (Right)  
- c2 — Talking on Phone (Right)  
- c3 — Texting (Left)  
- c4 — Talking on Phone (Left)  
- c5 — Operating Radio  
- c6 — Drinking  
- c7 — Reaching Behind  
- c8 — Hair & Makeup  
- c9 — Talking to Passenger  

---

## Tech Stack
- Python  
- TensorFlow / Keras  
- NumPy, Pandas  
- Matplotlib  
- Scikit-learn  

---

## Exploratory Data Analysis
- Checked class distribution (balanced dataset)  
- Visualized image samples  
- Analyzed subject-wise data  

Insight:
- Average images per class ≈ 2242  
- No major class imbalance  

---

## Model Architecture
- ResNet50 (Transfer Learning)

Configuration:
- Epochs: 10  
- Batch Size: 32  
- Optimizer: Adam  
- Loss: Categorical Crossentropy  

---

## Results

| Metric | Value |
|--------|------|
| Training Loss | 0.93 |
| Validation Loss | 3.79 |
| Holdout Loss | 2.64 |

Note:
- Slight overfitting due to limited hyperparameter tuning  

---

## Workflow
Data Collection → Preprocessing → EDA → Model Building → Training → Evaluation  

---

## Key Features
- Multi-class image classification  
- Deep learning pipeline  
- Real-world safety application  
- End-to-end implementation  

---

## Challenges
- High computational cost  
- Limited tuning resources  
- Overfitting on validation data  

---

## Future Improvements
- Hyperparameter tuning  
- Data augmentation  
- Fine-tuning pre-trained models  
- Deploy using Streamlit  

---

## Conclusion
This project demonstrates how Deep Learning can enhance road safety by identifying distracted driving behaviors. With further optimization, it can be deployed in real-time driver monitoring systems.
