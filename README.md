# 🏨 Customer Retention and Dynamic Pricing Analysis

> A data science project analyzing hotel booking patterns to reduce cancellations and optimize revenue through dynamic pricing strategies.

---

## 📌 Project Overview

In the highly competitive travel and hospitality sector, hotels suffer from significant revenue leakage due to unoptimized pricing and unpredictable customer cancellations. This project analyzes historical hotel booking data to:

- Uncover the **primary drivers of customer cancellations (churn)**
- Explore **seasonal demand trends**
- Build a foundation for a **dynamic pricing engine**
- Enable **targeted customer retention campaigns**

The dataset used is the [Hotel Booking Demand Dataset](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) containing 119,390 booking records across a Resort Hotel and a City Hotel, covering bookings from July 2015 to August 2017.

**Key Business KPIs:**
- Reduce overall cancellation rate
- Optimize Revenue Per Available Room (RevPAR)
- Improve Average Daily Rate (ADR) forecasting

---

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Data Processing & EDA | Python (Pandas, NumPy) |
| Visualization | Matplotlib, Seaborn |
| Predictive Modeling | Scikit-Learn |
| Dashboard | Tableau / Power BI |
| Version Control | Git & GitHub |
| Environment | Jupyter Notebook (Anaconda) |

---

## 📁 Repository Structure

```
Customer-Retention-and-Dynamic-Pricing-Analysis/
│
├── data/
│   ├── hotel_bookings.csv               # Raw dataset
│   └── hotel_bookings_cleaned.csv       # Cleaned dataset (Week 1 output)
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb           # Week 1 - Data Cleaning & Feature Engineering
│   ├── 02_eda.ipynb                     # Week 2 - Exploratory Data Analysis
│   ├── 03_predictive_modeling.ipynb     # Week 3 - Churn Prediction Model
│   └── 04_insights_summary.ipynb        # Week 4 - Final Insights
│
├── dashboard/
│   └── seasonal_pricing_dashboard.pbix  # Power BI / Tableau Dashboard
│
└── README.md
```

---

## ⚙️ How to Run

### Prerequisites
Make sure you have the following installed:
- [Anaconda](https://www.anaconda.com/download)
- Python 3.8+
- Required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/mg68339/Customer-Retention-and-Dynamic-Pricing-Analysis.git
cd Customer-Retention-and-Dynamic-Pricing-Analysis
```

**2. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

**3. Download the dataset**

Download `hotel_bookings.csv` from [Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) and place it in the `data/` folder.

**4. Launch Jupyter Notebook**
```bash
jupyter notebook
```

**5. Run notebooks in order**
- Start with `notebooks/01_data_cleaning.ipynb`
- Run each notebook from top to bottom in sequence

---

## 📊 Results & Findings

> ⚠️ This section will be updated as the project progresses week by week.

### ✅ Week 1 — Data Cleaning & Feature Engineering (Complete)

- Loaded dataset with **119,390 records** and **32 columns**
- Handled missing values:
  - `children` (4 missing) → filled with `0`
  - `country` (488 missing) → filled with `'Unknown'`
  - `agent` (16,340 missing) → filled with `0` (no agent used)
  - `company` (112,593 missing) → filled with `0` (no company used)
- Removed **negative ADR** values (data errors)
- Removed **ADR outlier** of 5,400 — extreme anomaly far beyond normal range
- Engineered new feature: `total_nights = stays_in_weekend_nights + stays_in_week_nights`
- Final cleaned dataset: **119,388 records**, saved as `hotel_bookings_cleaned.csv`

### 🔄 Week 2 — Exploratory Data Analysis (In Progress)
- Correlation matrix analysis
- Cancellation rate by lead time, deposit type, customer type
- ADR trends by month and season

### ⏳ Week 3 — Predictive Modeling (Upcoming)
- Logistic Regression / Decision Tree for cancellation prediction
- Evaluation: Accuracy, Precision, Recall, ROC-AUC

### ⏳ Week 4 — Dashboard & Presentation (Upcoming)
- Seasonal pricing dashboard in Tableau / Power BI
- Business recommendations for Revenue Management team

---

## 📬 Contact

For any queries related to this project, please reach out via the GitHub repository.

---

*This project was developed as part of a data science internship program focusing on Travel, Tourism & Hospitality analytics.*
