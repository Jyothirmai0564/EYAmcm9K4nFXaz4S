# 🔍 Predicting Term Deposit Subscriptions for a European Bank — ML Project at Apziva

[![Repo Link](https://img.shields.io/badge/GitHub-Repository-blue)](https://github.com/Jyothirmai0564/EYAmcm9K4nFXaz4S)

## 📌 Project Summary

As part of my data science training at **Apziva**, I worked on a real-world project where I developed a complete machine learning pipeline for a European bank's marketing campaign. The bank's objective was to **improve term deposit subscription rates** through efficient customer targeting, reduce wasted outbound calls, and optimize follow-up strategies.

My project addresses this through:

- A **Pre-Call Classifier** to avoid calling unlikely subscribers.
- A **Post-Call Classifier** to detect potential converters among initial “No” respondents.
- A **Customer Segmentation Model** using PCA + KMeans to aid campaign strategy.
- Detailed **EDA, feature importance analysis**, and **business recommendations**.

## 🚀 Step-by-Step Project Workflow

### 1. **Business Understanding & Objective Framing**

- Goal: Increase conversion in term deposit marketing campaigns.
- Challenges:
  - High call costs.
  - Low response rates.
  - Need to prioritize which customers to call or follow up with.

---

### 2. **Data Preprocessing & EDA**

- **Dataset**: Bank marketing dataset with 45,000+ records.
- **Techniques**:
  - Missing value handling.
  - Label encoding for categorical variables.
  - Outlier detection and distribution analysis.
- **Key Insights**:
  - Call duration was highly indicative of conversions.
  - Certain months like March and October had better response rates.
  - Customers without housing/loan obligations were more flexible.

---

### 3. **Pre-Call Subscription Prediction**

- **Model Objective**: Predict whether a customer will say **“Yes” or “No”** before the call.
- **Best Model**: `XGBoost`
- **Performance**:
  - Skipped ~9,426 unlikely customers.
  - Saved ~785.5 hours of call time.
  - Achieved >81% accuracy threshold via cross-validation.
- **Top Features**: `age`, `balance`, `loan`, `housing`, `education`, `job`

---

### 4. **Post-Call Follow-Up Prediction**

- **Model Objective**: Identify potential subscribers **after an initial “No”**.
- **Best Model**: `LightGBM` (AUC: 0.9971)
- **Alternate Models**: `Bagging` (best recall), `AdaBoost` (aggressive follow-up).
- **Outcome**:
  - 1,221 high-likelihood converters identified.
  - Balanced recall, precision, and minimal false negatives.
- **Key Features**:
  - `total_contact_time`, `contact_intensity`, `campaign`, `month`, `call_duration`

---

### 5. **Customer Segmentation (Clustering)**

- **Goal**: Group customers into meaningful clusters for tailored outreach.
- **Techniques**:
  - PCA (Explained Variance ~79.3% from top 3 components).
  - KMeans (Optimal K = 7, Silhouette Score = 0.59).
- **Cluster Interpretation**:

| Cluster | Segment             | Traits                                    | Subscription Rate |
|--------:|---------------------|-------------------------------------------|-------------------|
| 6       | 🟢 High Value        | Long, focused calls; fewer touches        | **7.1%**          |
| 1       | 🟡 Easy Wins         | Convert with minimal effort               | 5.2%              |
| 0       | 🟠 Moderate          | Many touches, moderate outcome            | 6.8%              |
| 5       | 🔴 Resource Drain    | Excessive contact, low return             | 6.6%              |
| 4       | ❌ Inefficient        | Long calls, many contacts, poor return    | **4.9%**          |
| 3       | ❌ Low-Value         | Fast decisions or disinterest             | **4.8%**          |
| 2       | ⚠️ High Effort        | High call time, low ROI                   | 5.6%              |

---

## 📌 Key Contributions

- Built a **two-phase classification system** that achieved industry-relevant efficiency improvements.
- Created a **PCA-based customer segmentation model** with business-actionable clusters.
- Performed **feature importance analysis** to support interpretability and strategy.
- Delivered **business recommendations** based on model and cluster insights.

---

## 📊 Visual Outputs

- ROC Curves for Pre- and Post-Call models.
- 3D PCA Cluster Plot.
- Feature importance bar plots.
- Silhouette Analysis for clustering validation.

---

## 💼 Final Remarks for Recruiters & Hiring Managers

This project showcases my **end-to-end machine learning capability**, from data wrangling and modeling to evaluation and interpretation. I’ve not only built high-performing models but also ensured **business alignment**, **explainability**, and **actionable insights** for strategic marketing decisions.

**✅ Achievements**:
- Surpassed 81% accuracy threshold.
- Identified over 1,200 follow-up candidates.
- Performed customer segmentation to support campaign design.

I’m excited to bring these skills into real-world data science roles focused on customer analytics, predictive modeling, and business impact.

---

## 📎 GitHub Repository

🔗 [Project Repo on GitHub](https://github.com/Jyothirmai0564/EYAmcm9K4nFXaz4S)

---

## 🧑‍💼 Author

**Jyothirmai**
- Data Science Trainee at Apziva
- 📫 [LinkedIn / Email — Insert if public]

---


