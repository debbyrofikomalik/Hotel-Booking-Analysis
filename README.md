# Project 1: Hotel Booking Cancellation Analysis

This project presents a comprehensive analysis of hotel booking data aimed at identifying factors contributing to high cancellation rates for both **City Hotels** and **Resort Hotels**. The insights derived are used to propose actionable recommendations for reducing cancellations, optimizing room utilization, and maximizing revenue.

---

## Project Overview

In recent years, City Hotels and Resort Hotels have experienced high cancellation rates. As a result, both types of hotels face several challenges, including reduced revenue and suboptimal room utilization. Reducing cancellation rates has therefore become a primary objective to enhance operational efficiency and maximize revenue generation. This analysis provides a data-driven approach to understand the key factors affecting booking cancellations and offers strategies to mitigate financial risk.

### Key Objectives
The analysis addresses the following research questions:
* What variables affect hotel reservation cancellations?
* How can hotel reservation cancellations be reduced?
* How can hotels be supported in making pricing and promotional decisions?

### Hypotheses
The following initial hypotheses were explored:
* Higher prices lead to more cancellations.
* Longer waiting lists increase the likelihood of cancellations.
* Most clients make reservations through offline travel agents.

---

## Dataset Overview

The dataset contains **119,390 observations** for a City Hotel and a Resort Hotel. Each entry corresponds to a single booking made between **July 1, 2015, and August 31, 2017**, including reservations that were completed and those that were canceled. It is publicly available on Kaggle.  

### Tools and Technologies
* **Programming Language:** Python (Google Colab)  
* **Libraries:** `pandas`, `matplotlib`, `seaborn` (used for Data Cleaning, EDA, and Visualization)

### Data Cleaning and Pre-processing
* **Personally Identifiable Information (PII) Removal:** Columns containing sensitive PII (**name, email, phone number, credit card**) were removed, reducing the dataset from 36 to 32 columns.  
* **Data Type Correction:** The **reservation_status_date** column was converted to datetime format for time-based analysis.  
* **Handling Missing Values:**  
  - The **company** column, with over 95% missing values, was dropped.  
  - Columns with smaller missing values (**children, country, agent**) were handled by removing the corresponding rows.  
* **Outlier Treatment:** Rows with extreme outliers in the **Average Daily Rate (ADR)** (ADR ≥ 5000) were removed to ensure representative analysis.

---

## Key Findings and Insights

### Overall Cancellation Rate
* **37.1%** of all clients canceled their reservations, significantly impacting hotel revenue.  
* **62.9%** of reservations remained confirmed.

### Cancellation Trends by Hotel Type
* **City Hotels** have more bookings overall than Resort Hotels.  
* The absolute number of cancellations is higher in **City Hotels**, though relative cancellation rates may indicate concerns for Resort Hotels.

### Factors Influencing Cancellation
* **Price (Average Daily Rate - ADR):** Higher ADR is associated with a higher likelihood of cancellation.  
* **Timing (Month):**  
  - Both confirmed and canceled reservations peak in August.  
  - January records the highest volume of cancellations.  
* **Market Segment:** The largest proportion of guests book through **Online Travel Agencies (47%)**, followed by Offline TA/TO (20%) and Groups (17%).  
* **Geographic Origin:** **Portugal (PRT)** has the highest number of cancellations among all countries.

---

## Recommendations

The following recommendations are proposed to reduce cancellations and maximize revenue:

| Key Insight | Recommendation | Strategic Objective |
| :--- | :--- | :--- |
| Cancellation rates rise with higher prices | Adjust pricing strategies by offering **location-based rate reductions** and targeted **discounts** | Reduce price sensitivity and incentivize retention |
| High cancellations in January | Launch targeted **marketing campaigns or special promotions** in January | Capitalize on low-demand/high-cancellation periods |
| Higher cancellations in Resort Hotels | Offer **discounted room rates** during weekends or holidays | Address seasonal/peak pricing sensitivity |
| Portugal is the top country for cancellations | Enhance **hotel quality and service standards** for bookings from Portugal | Improve perceived value to reduce risk of cancellation |

For a more detailed explanation, visualizations, and methodology, see the [deck presentation](https://example.com).
