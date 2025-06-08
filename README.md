# Machine Learning: Mobile Plan Recommendation

This project aims to help the mobile operator **Megaline** recommend a more suitable plan (Smart or Ultra) to their users, based on their monthly behavior. Using behavioral data from existing users, we built a classification model that predicts the most appropriate plan.

## 📁 Project Files

- `Machine_Learning.ipynb` — main analysis notebook
- `datasets/users_behavior.csv` — user activity data

## 🧠 Project Overview

- **Goal:** Build a model that predicts whether a user should switch to the Ultra or Smart plan.
- **Target metric:** Accuracy ≥ 0.75
- **Target variable:** `is_ultra` (1 = Ultra, 0 = Smart)

### Dataset Features:

- `calls` — number of calls per month
- `minutes` — total call duration
- `messages` — number of text messages
- `mb_used` — mobile internet usage in MB
- `is_ultra` — current plan (target)

## 🛠️ Methodology

1. Split the dataset into **training**, **validation**, and **test** sets
2. Trained and evaluated several models:
   - Decision Tree
   - Random Forest
   - Logistic Regression
3. Tuned hyperparameters for best performance
4. Validated final model on the test set

## ✅ Results

- **Logistic Regression** showed the lowest accuracy
- **Decision Tree** performed reasonably well with fast training time
- **Best model:** **Random Forest** (20 trees, max depth = 6)
  - Achieved **accuracy above 0.75** on the test set

## 📌 Conclusion

Random Forest provided the most accurate predictions and is recommended for implementation. This model can help Megaline efficiently suggest the best mobile plan based on user behavior.

