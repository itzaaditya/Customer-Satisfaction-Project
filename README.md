# ✈️ Customer Satisfaction Prediction using Machine Learning

This project uses machine learning techniques to predict customer satisfaction levels for an airline based on various in-flight and service-related features.

---

## 📂 Dataset

Source: [Customer Feedback and Satisfaction - Kaggle](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction)

The dataset includes passenger information, service ratings (e.g., inflight wifi, food, cleanliness), delays, and the target label: **Satisfaction** (`satisfied` vs `neutral_or_dissatisfied`).

---

## 🔍 Objective

To build a classification model that predicts customer satisfaction using the following algorithms:

- Logistic Regression (with GridSearchCV for tuning)
- Random Forest
- Support Vector Machine (SVM)

---

## 🧰 Features Used

- Gender, Age, Customer Type, Travel Class
- Flight Distance, Departure/Arrival Delay
- Service Ratings: Online booking, Inflight Wifi, Seat Comfort, Food, Cleanliness, etc.
- Engineered Features: Delay Ratio, Average Rating, Binary Delay flag

---

## ✅ ML Pipeline

1. **Data Cleaning**
   - Lowercasing and replacing spaces in categorical columns
   - Handling missing values (`arrival_delay_in_minutes`)
2. **Preprocessing**
   - One-hot encoding with `DictVectorizer`
   - Normalizing numerical features with `StandardScaler`
3. **Modeling**
   - Logistic Regression with `GridSearchCV`
   - Random Forest Classifier
   - Support Vector Classifier (SVC & LinearSVC)
4. **Evaluation**
   - Accuracy
   - F1 Score
   - Confusion Matrix

---

## 🔎 Results

| Model                       | Accuracy | F1 Score |
| --------------------------- | -------- | -------- |
| Logistic Regression (Tuned) | 85%      | 0.84     |
| Random Forest               | 96%      | 0.96     |
| SVM (LinearSVC)             | 83%      | 0.82     |

---

## 📝 How to Run

```bash
# Create environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows use venv\Scripts\activate

# Install requirements
pip install -r requirements.txt

# Run the notebook
jupyter notebook
```
