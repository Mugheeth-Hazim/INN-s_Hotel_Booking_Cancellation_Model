# INN Hotels – Booking Cancellation Prediction

This notebook looks at hotel reservation data and tries to understand what drives cancellations. It goes through a full analysis of guest behavior, booking patterns, and then builds predictive models to classify which bookings are more likely to be canceled.

---

## Project Goals

The aim was to explore how different features like booking dates, guest type, room preferences, and other signals might impact the likelihood of a cancellation. Based on that, models were trained to try and flag risky bookings ahead of time.

---

## Key Steps in the Notebook

### 🧹 Data Cleaning

- Dropped the Booking ID column (it doesn’t add value for prediction).
- Looked at missing values and column types.
- No major issues were found, so the dataset was ready to explore.

### 📊 EDA (Exploratory Data Analysis)

The notebook asks a few practical questions, like:

- What months have the most bookings?
- Which guest segments cancel the most?
- Do repeat guests cancel less?
- Are people with special requests more or less likely to cancel?

From this, we learn things like:
- Most guests come in peak months (based on monthly booking count).
- Corporate and online guests behave differently.
- Cancellation rate is noticeably lower for repeat customers.
- Some patterns, like lead time or total nights, seem to impact cancellation rates too.

### 📈 Modeling

Two types of classification models were trained:

1. **Logistic Regression** – A baseline model to understand the data better.
2. **Decision Tree** – To capture non-linear patterns.

The performance was measured using:
- Accuracy
- AUC (Area Under the ROC Curve)
- Confusion Matrix
- Precision & Recall

Some tuning was done to improve the results slightly, especially for the tree model.

---

## Tools Used

- Python (Pandas, NumPy, Seaborn, Matplotlib)
- Scikit-learn for machine learning
- Jupyter Notebook

---

## Business Insights

- Repeat guests are more reliable.
- Certain market segments have higher cancellation rates.
- Special requests might indicate more commitment (lower cancellation rate).
- These models can help hotels flag bookings that are likely to be canceled and take action early.

---

## What's Next?

Some ideas to take this further:
- Try ensemble models like Random Forests
- Tune hyperparameters more aggressively
- Add external signals like holidays or weather
- Build a dashboard for hotel staff to use this in real-time

---

## Files

- `INNHotels_Booking_Cancelation_Model.ipynb`: Full analysis and model code
- `README.md`: This file
