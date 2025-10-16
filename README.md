# Hotel Booking Analysis using Python

## 📘 Project Overview

This project focuses on analyzing hotel booking data from a **City Hotel** and a **Resort Hotel** to understand the factors driving high cancellation rates and provide actionable recommendations to minimize cancellations and maximize revenue.  
Both hotels have faced challenges such as **reduced revenue** and **underutilized room capacity** due to high cancellation rates.

This analysis was conducted as part of a **Data Analysis Portfolio Project**, using **Python (Google Colab)** for data cleaning and exploratory data analysis (EDA), and **Power BI** for potential dashboard visualization.

---

## 🗂️ Table of Contents
1. [Business Problem](#business-problem)  
2. [Assumptions](#assumptions)  
3. [Research Questions & Hypotheses](#research-questions--hypotheses)  
4. [Data Source & Dictionary](#data-source--dictionary)  
5. [Tools and Technologies](#tools-and-technologies)  
6. [Data Analysis and Key Findings](#data-analysis-and-key-findings)  
7. [Recommendations](#recommendations)  
8. [Access Code](#access-code)

---

## 💼 Business Problem

In recent years, both **City Hotel** and **Resort Hotel** have been facing **high cancellation rates**, resulting in **revenue loss** and **inefficient room utilization**.  
The objective of this project is to identify the factors influencing these cancellations and to develop data-driven strategies to reduce them, improve efficiency, and increase profitability.

---

## 📋 Assumptions

- Events between 2015 and 2017 do not significantly impact the dataset.  
- The data remains relevant for current hotel operations.  
- The recommended strategies will not lead to negative business impacts.  
- The hotels are not yet applying these recommendations.  
- Booking cancellations significantly affect hotel revenue.  
- Most bookings and cancellations occur within the same year.

---

## ❓ Research Questions & Hypotheses

### Research Questions
1. What variables influence hotel reservation cancellations?  
2. How can hotels minimize reservation cancellations?  
3. How can pricing and promotional strategies be optimized?

### Hypotheses
1. Cancellation rates increase with higher **Average Daily Rate (ADR)**.  
2. Longer **waiting lists** lead to more frequent cancellations.  
3. **Offline travel agents** contribute more reservations than online channels.

---

## 📊 Data Source & Dictionary

The dataset includes **119,390 hotel bookings** from a **City Hotel** and a **Resort Hotel**, covering **July 2015 – August 2017**.  
It contains both completed and canceled reservations and is available on **Kaggle**:  
🔗 [Hotel Booking Demand Dataset](https://www.kaggle.com/datasets/mojtaba142/hotel-booking/data)

### Key Columns

| Column | Description |
| :--- | :--- |
| `hotel` | Type of hotel (City Hotel or Resort Hotel) |
| `is_canceled` | Indicates whether the booking was canceled (1) or not (0) |
| `lead_time` | Days between booking date and arrival date |
| `market_segment` | Booking source (Travel Agents, Tour Operators, etc.) |
| `deposit_type` | Deposit status (No Deposit, Non Refund, Refundable) |
| `days_in_waiting_list` | Number of days booking stayed on waiting list |
| `adr` | Average Daily Rate – total lodging revenue / total nights stayed |
| `total_of_special_requests` | Number of special requests made |
| `country` | Country of origin of the guest |
| `reservation_status` | Final status (Checked-Out, Canceled, No-Show) |

---

## 🧰 Tools and Technologies

- **Programming Language:** Python  
- **Environment:** Google Colab  
- **Libraries:** Pandas, Matplotlib, Seaborn  
- **Visualization:** Power BI, Canva  
- **Skills:** Data Cleaning, Exploratory Data Analysis (EDA), Data Visualization  

---

## 📈 Data Analysis and Key Findings

### 1. Overall Cancellation Rate
- **37.1%** of all bookings were canceled — a major impact on hotel revenue.  
- **City Hotels** have more bookings but also higher cancellation rates than Resort Hotels.

### 2. Price (ADR) and Cancellations
- Cancellations are **more frequent when ADR is higher**, showing that **price sensitivity** is a major factor.  
- The highest ADR for canceled bookings occurs in **January**, while **August** records the most cancellations overall.

### 3. Monthly Trends
- Both confirmed and canceled reservations **peak in August**.  
- **January** consistently shows the **highest cancellation volume**.

### 4. Cancellations by Country
- **Portugal (PRT)** has the highest number of canceled bookings compared to other countries.

### 5. Booking Source Distribution
- **Online Travel Agencies (47%)** dominate booking sources.  
- **Groups (27%)** follow, while **Direct bookings (4%)** are minimal.

---

## 💡 Recommendations

| Key Finding | Recommendation | Objective |
| :--- | :--- | :--- |
| High cancellations at high ADR | Implement **dynamic and targeted pricing strategies** to address price sensitivity. | Reduce cancellations caused by high prices. |
| January as peak cancellation month | Run **promotional campaigns and discounts** in January. | Improve room occupancy and stabilize revenue. |
| Higher cancellations in Resort Hotels | Offer **special weekend and holiday discounts**. | Increase occupancy and reduce seasonal cancellations. |
| Portugal as top cancellation country | **Enhance service quality** and improve communication with Portuguese guests. | Minimize cancellations from this key market. |

---

## 💻 Access Code

The Python notebook used for cleaning, analysis, and visualization can be accessed below:  
🔗 [Open in Google Colab](https://colab.research.google.com/drive/1lSOFX6ZmrgjszC-u14KHjPdHcu5PJjZX?usp=sharing)

---

## 👩‍💻 Author
**Debby Rofiko Malik**  
🎓 Biomedical Engineering, Universitas Indonesia  
📧 [debbymalik21@gmail.com](mailto:debbymalik21@gmail.com)  
💼 [LinkedIn](https://www.linkedin.com/in/debby-rofiko-malik/)  
🌐 [GitHub](https://github.com/debbyrofikomalik)
