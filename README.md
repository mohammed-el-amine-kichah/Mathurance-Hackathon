# 🧠 Mathurance Hackathon — Claims Triangle Prediction

This project was developed during the **Mathurance Hackathon 2025**, a data science competition focused on insurance analytics. Our goal was to **predict the lower triangle of a claims development triangle**, a common challenge in actuarial science.

---

## 📊 Problem Statement

Insurance claims are typically reported and settled over several years. These are summarized in a **claims development triangle**, where:

- **Rows** represent accident years,
- **Columns** represent development years,
- The **upper triangle** contains observed data,
- The **lower triangle** contains future (unknown) claim amounts we aim to predict.

---

## 🔧 Our Approach

We combined traditional actuarial modeling with deep learning to enhance prediction accuracy:

### 1. 🧮 Chain Ladder Method
- Applied the classical **Chain Ladder algorithm** to generate initial forecasts.
- Assumes a consistent development factor between years.
- Offers **strong interpretability** and is widely used in insurance.

### 2. 🤖 LSTM (Long Short-Term Memory)
- Trained an **LSTM model** on historical claim patterns to capture **non-linear temporal dependencies**.
- Reshaped the triangle into sequences and trained the model to predict future developments.
- Helped capture **complex trends** and anomalies missed by Chain Ladder.

---

## 📈 Results

- **Chain Ladder** provided a solid baseline with high interpretability.
- **LSTM** captured subtler temporal patterns and improved accuracy in volatile scenarios.
- **Final predictions** combined insights from both models for better robustness and performance.

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- TensorFlow
- Matplotlib / Seaborn

