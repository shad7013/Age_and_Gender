# Age & Gender Prediction (Kaggle Competition)

##  Overview
This project focuses on predicting **age (regression)** and **gender (classification)** from facial images using deep learning.  
It was developed as part of a Kaggle competition with a multi-task learning approach.

---

##  Approach
- Built a **custom CNN from scratch** for joint age and gender prediction  
- Improved performance using **transfer learning (ResNet50)**  
- Handled **class imbalance** using weighted sampling and class-weighted loss  
- Applied **data augmentation and normalization** for better generalization  

---

##  Model Details
- **Framework:** PyTorch  
- **Tasks:**
  - Age → Regression (L1 Loss)
  - Gender → Classification (CrossEntropy Loss)  
- **Multi-task learning:** Shared backbone with separate heads  
- **Evaluation Metric:** Harmonic Mean of F1 Score (gender) and nRMSE (age)

---

##  Pipeline
1. Data loading & preprocessing  
2. Train-validation split (stratified)  
3. Model training (CNN + ResNet50)  
4. Experiment tracking using TrackIO  
5. Model saving via Kaggle Hub  
6. Inference and submission generation  

---

##  Results
- Scratch CNN achieved a leaderboard score of **0.46**  
- Performance improved using fine-tuned ResNet50  

---

##  Output
- Final predictions saved as `submission.csv`  
- Format:
