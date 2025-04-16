# AddictoScope

AddictoScope is a machine learning project aimed at predicting social media addiction levels using behavioral and demographic data. By analyzing patterns like watch time, platform preference, and frequency of use, it leverages models like Random Forest, XGBoost, and Neural Networks to detect signs of digital addiction.

## Project Goal
The goal of this project is to build an end-to-end machine learning pipeline that identifies and predicts an individual's addiction level to social media. It aims to uncover behavioral patterns that contribute to digital overuse and provide insights into user engagement habits.

## Dataset Info
**Source:** Custom dataset titled `Time-Wasters on Social Media_ML.csv`

### Features:

**Categorical:**
- Gender
- Location
- Profession
- Platform
- Device Type
- OS
- Connection Type
- Watch Reason
- Current Activity
- Video Category
- Frequency

**Numerical:**
- Age
- Watch Time (converted to minutes)

**Target:**
- Addiction Level

### Preprocessing:
- Dropped missing values and irrelevant columns (e.g., UserID)
- Label encoding and scaling applied to appropriate features
- Watch Time converted from time format to minutes

## Models Used
- **Linear Regression**
- **Random Forest Regressor**
- **XGBoost Regressor**
- **Neural Network** using TensorFlow/Keras

All models were trained and evaluated using:
- R² Score
- Mean Squared Error (MSE)

## Insights & Findings
Key features contributing to high addiction levels include:
- **Watch Time**
- **Platform and Device Type**
- **Video Category and Frequency of usage**

**XGBoost** and **Neural Networks** showed the highest predictive performance among all models.

Feature importance analysis helped in identifying behavioral patterns correlated with addictive use.

## How to Run

```bash
# Clone the repository
git clone https://github.com/ssg2005/addicto-scope.git
cd addictoscope

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook
