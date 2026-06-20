# 🚗 Rides Data Analysis — Portfolio Project

**Objective:** Analyze ride-sharing data to uncover patterns, improve customer satisfaction, and enhance operational efficiency.

---

## 📁 Project Structure

| File | Description |
|---|---|
| `rides_data.csv` | Synthetic dataset — 5,000 rides across 5 Indian cities (2024) |
| `rides_analysis.ipynb` | Full analysis notebook — EDA, demographics, clustering |
| `fig1_operations.png` | Operations dashboard — peak hours, revenue, city breakdown |
| `fig2_demographics.png` | Demographics — age, gender, payment, segments |
| `fig3_clustering.png` | K-Means clustering — 4 user segments |

---

## 📊 Dataset Overview

| Column | Description |
|---|---|
| ride_id | Unique ride identifier |
| user_id | User identifier (1–2000) |
| timestamp | Date and time of ride |
| city | One of 5 Indian metros |
| ride_type | Standard / Premium / Pool / XL |
| distance_km | Trip distance |
| duration_min | Trip duration |
| base_fare | Fare before surge |
| surge_multiplier | 1.0 / 1.5 / 2.0 |
| final_fare | Actual amount charged |
| rating | 1–5 star rating |
| payment_method | UPI / Card / Cash / Wallet |
| cancelled | 0 = completed, 1 = cancelled |
| user_age | Rider age (18–65) |
| user_gender | Male / Female / Other |
| user_segment | Student / Young Professional / Mid-Career / Senior |
| is_peak_hour | 1 if 7–9 AM or 5–8 PM |

---

## 🔍 Key Findings

### Operations
- **Peak demand** occurs at 7–9 AM and 5–8 PM — 45% of all rides happen in these windows
- **Mumbai** generates ~30% of total revenue — highest priority market
- **Peak-hour fares** are ~25% higher due to surge pricing

### User Demographics
- **Young Professionals (26–35)** are the largest rider segment by volume
- **Mid-Career users (36–50)** have the highest average spend per ride (₹158)
- **UPI is dominant** at 45% — strong opportunity for loyalty programs

### User Clustering (K-Means, k=4)
| Cluster | Avg Rides | Avg Fare | Cancel Rate | Strategy |
|---|---|---|---|---|
| Frequent Riders | 4.5 | ₹146 | 6% | Loyalty rewards, subscriptions |
| Premium Riders | 2.4 | ₹319 | 6% | Upsell XL, premium perks |
| Churners | 2.4 | ₹112 | 54% | Discount vouchers, push notifications |
| Occasional Riders | 2.0 | ₹87 | 0% | First-ride offers, referral codes |

---

## 💡 Business Recommendations

1. **Dynamic pricing** — Implement 1.5× surge during peak windows to boost revenue by 15–20%
2. **Churn intervention** — Target Churner cluster with personalised discounts — estimated 15% win-back
3. **Mumbai-first expansion** — Increase driver supply during peak hours to reduce wait time
4. **UPI cashback partnerships** — Collaborate with PhonePe or Google Pay for the 26–35 segment
5. **Premium loyalty tier** — Subscription plan for Premium Riders with priority pickup and no surge

---

## 🛠 Tools Used
- **Python** — Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Machine Learning** — K-Means Clustering, PCA
- **Environment** — Jupyter Notebook (Anaconda)

---

*Built as a portfolio project to demonstrate end-to-end data analysis skills for a Business/Marketing Analyst role.*
