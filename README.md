# Predictive Analytics of Hotel Booking Cancellations

Predictive analytics project to forecast hotel booking cancellations using decision tree and random forest models.

---

## 📌 Problem Statement

Hotel booking cancellations pose a significant challenge for revenue management and operational planning in the hospitality industry.  
The objective of this project is to develop a predictive model capable of identifying hotel reservations with a high probability of cancellation, enabling data-driven decision-making.

This work applies data science and machine learning techniques to analyze booking behavior and uncover the most influential factors behind reservation cancellations.

---

## 📊 Dataset

The analysis is based on the **Hotel Booking Demand** dataset, which contains **119,390 records and 32 variables** related to hotel reservations between 2015 and 2017.

**Key features include:**
- Booking lead time
- Deposit type
- Average daily rate (ADR)
- Customer and market segment information
- Special requests and parking requirements

Dataset source (public):
https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand

🧪 Methodology

The analytical workflow follows a structured, end-to-end data science pipeline:

Exploratory Data Analysis (EDA)

Descriptive statistics

Correlation analysis (full and filtered matrices)

Visual analysis of key predictors

Data Preprocessing

Handling missing values

Encoding categorical variables

Stratified train-test split (80/20)

Predictive Modeling

Decision Tree classifiers with progressive feature inclusion

Hyperparameter optimization using GridSearchCV

Ensemble modeling with Random Forest

Model Evaluation

Accuracy, Precision, Recall, F1-Score

ROC-AUC

Confusion matrices (raw and normalized)

📈 Key Results

Deposit type and lead time emerged as the most influential predictors of cancellation.

Models combining numerical and categorical features significantly outperformed simpler specifications.

The Random Forest model achieved the best overall performance, with higher accuracy and precision compared to optimized decision trees.

The final models demonstrate strong capability to distinguish between canceled and non-canceled reservations in a class-imbalanced setting.

Detailed results, figures, and discussion are available in the full report:

reports/predictive-analytics-hotel-booking-cancellations.pdf

📁 Repository Structure
hotel-booking-cancellation-prediction/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── 00_end_to_end_hotel_booking_cancellations.ipynb
├── figures/
├── reports/
│   └── predictive-analytics-hotel-booking-cancellations.pdf
├── src/
├── README.md
├── requirements.txt
└── LICENSE

▶️ How to Run

Clone the repository

Install dependencies:

pip install -r requirements.txt


Place the dataset in:

data/raw/hotel_bookings.csv


Run the notebook:

notebooks/00_end_to_end_hotel_booking_cancellations.ipynb

⚠️ Notes and Limitations

The analysis relies exclusively on booking-level data and does not include external economic or behavioral variables.

Future work may incorporate macroeconomic indicators or customer sentiment analysis to further enhance predictive performance.

👤 Author

Julián Alberto Delgadillo Marín
M.Sc. in Applied Economics (candidate)
University of Buenos Aires (UBA)

