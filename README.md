# Hotel Booking 

## Project Overview

This project focuses on analyzing hotel booking data from a City Hotel and a Resort Hotel to understand the factors driving high cancellation rates and provide actionable recommendations to minimize cancellations and maximize revenue. The initial problem statement highlights that both hotels face significant challenges, including reduced revenue and suboptimal room utilization, due to these high cancellation rates.

This analysis was performed as a Data Analysis portfolio project, utilizing **Python** (specifically in a Google Colab environment) for data cleaning and exploratory data analysis (EDA), and **Power BI** for potential dashboarding (though the primary analysis presented is in Python).

## Table of Contents

1.  [Business Problem](#business-problem)
2.  [Assumptions](#assumptions)
3.  [Research Questions & Hypotheses](#research-questions--hypotheses)
4.  [Data Source & Dictionary](#data-source--dictionary)
5.  [Tools and Technologies](#tools-and-technologies)
6.  [Data Analysis and Key Findings](#data-analysis-and-key-findings)
7.  [Recommendations](#recommendations)
---

## Business Problem

[cite_start]In recent years, both **City Hotel** and **Resort Hotel** have been struggling with **high cancellation rates**[cite: 36]. [cite_start]This phenomenon has led to negative consequences such as **reduced revenue** and **underutilized room capacity**[cite: 37]. [cite_start]The main objective of this project is to analyze the underlying patterns and variables that influence these cancellations, ultimately aiming to develop strategies to lower the cancellation rates, enhance efficiency, and maximize revenue generation for both hotels[cite: 38].

---

## Assumptions

[cite_start]The analysis is conducted under the following key assumptions[cite: 60, 61, 62, 63, 64, 65, 66, 67]:

* [cite_start]**Data Integrity:** No unusual occurrences between 2015 and 2017 substantially impacted the dataset[cite: 61].
* [cite_start]**Relevance:** The information remains relevant and can be applied to efficiently analyze potential hotel strategies[cite: 62].
* [cite_start]**Neutral Impact:** Implementing the suggested techniques is assumed to have no unforeseen negative consequences for the hotels[cite: 63].
* [cite_start]**Novelty of Solutions:** The hotels are not currently employing any of the suggested solutions[cite: 64].
* [cite_start]**Primary Factor:** Booking cancellations are the single biggest factor affecting the effectiveness of earning income[cite: 65].
* [cite_start]**Impact of Cancellation:** Cancellations result in vacant rooms for the booked length of time[cite: 66].
* [cite_start]**Booking Timeline:** Clients make hotel reservations and cancellations within the same year[cite: 67].

---

## Research Questions & Hypotheses

### Research Questions
1.  [cite_start]What variables affect hotel reservation cancellations[cite: 69]?
2.  [cite_start]How can hotel reservation cancellations be reduced[cite: 70, 71]?
3.  [cite_start]How can hotels be supported in making pricing and promotional decisions[cite: 72, 73]?

### Hypotheses
1.  [cite_start]**Price Effect:** More cancellations occur when prices (Average Daily Rate) are higher[cite: 76].
2.  [cite_start]**Waiting List Effect:** When there is a longer waiting list, customers tend to cancel more frequently[cite: 77, 78].
3.  [cite_start]**Source of Booking:** The majority of clients are coming from offline travel agents to make their reservations[cite: 79].

---

## Data Source & Dictionary

[cite_start]The dataset comprises **119,390** hotel bookings from a City Hotel and a Resort Hotel, covering reservations made between **July 1, 2015, and August 31, 2017**[cite: 40, 41]. [cite_start]The data includes both completed and canceled reservations and is available on Kaggle[cite: 41, 42].

### Key Columns (Variables)
| Column Name | Description |
| :--- | :--- |
| **hotel** | [cite_start]Indicates whether the booking was for a City Hotel or a Resort Hotel[cite: 44]. |
| **is\_canceled** | [cite_start]Shows whether the booking was canceled (1) or not (0)[cite: 44]. |
| **lead\_time** | [cite_start]Number of days between the booking date and the arrival date[cite: 44]. |
| **market\_segment** | [cite_start]Booking market segment (e.g., 'TA' for Travel Agents, 'TO' for Tour Operators)[cite: 49]. |
| **deposit\_type** | [cite_start]Type of deposit (No Deposit, Non Refund, Refundable)[cite: 55]. |
| **days\_in\_waiting\_list** | [cite_start]Number of days the booking was on the waiting list before confirmation[cite: 55]. |
| **adr** | [cite_start]**Average Daily Rate**, calculated by dividing total lodging revenue by the total number of nights stayed[cite: 58]. |
| **total\_of\_special\_requests** | [cite_start]Number of special requests made by the customer[cite: 58]. |
| **country** | Country of origin of the customer. |
| **reservation\_status** | [cite_start]Final booking status (Check-Out, Canceled, No-Show)[cite: 58]. |

---

## Tools and Technologies

* [cite_start]**Programming Language:** Python [cite: 31]
* [cite_start]**Environment:** Google Colab [cite: 31]
* [cite_start]**Skills Utilized:** Data Cleaning [cite: 31][cite_start], Exploratory Data Analysis [cite: 32][cite_start], Data Visualization [cite: 32]

---

## Data Analysis and Key Findings

### 1. Overall Cancellation Rate

* [cite_start]**Finding:** A total of **37.1%** of all clients canceled their reservations[cite: 440, 447, 450]. [cite_start]This is a substantial proportion that significantly impacts hotel revenue performance[cite: 450].
* [cite_start]**Hotel Comparison:** **City Hotels** have more bookings overall than Resort Hotels[cite: 476], but the proportion of cancellations in the City Hotel is also higher than in the Resort Hotel (visually observable from the bar chart on page 18).

### 2. The Influence of Price (ADR) on Cancellations

* [cite_start]**Finding:** Reservations are **more likely to be canceled when the Average Daily Rate (ADR) is higher**[cite: 530, 76]. [cite_start]Conversely, cancellations occur least frequently when prices are lowest[cite: 503]. [cite_start]This strongly suggests that the **accommodation cost is a main factor** influencing cancellations[cite: 504].
* [cite_start]**Monthly ADR:** The total ADR from canceled bookings **peaks in January** [cite: 488, 502][cite_start], despite August having the highest number of overall cancellations[cite: 480].

### 3. Monthly Cancellation Trends

* [cite_start]**Finding:** Both confirmed and canceled reservations **peak in August**[cite: 480].
* [cite_start]**Critical Month:** **January records the highest number of canceled reservations**[cite: 480]. This month represents a significant loss of potential revenue.

### 4. Top Cancellation Country

* [cite_start]**Finding:** **Portugal (PRT)** ranks first with the greatest number of reservation cancellations, far exceeding other countries[cite: 506, 526].

### 5. Booking Source Distribution

* [cite_start]**Finding:** The majority of guests book through **Online Travel Agencies (Online TA)**, accounting for approximately **47.4%** of bookings[cite: 483, 501].
* [cite_start]**Groups** account for about **16.7%** [cite: 483][cite_start], but the slide combines Online TA (47.4%) and Offline TA/TO (20.3%) and states that around 46% book through online travel agencies, 27% through groups, and only 4% make direct bookings[cite: 501].

---

## Recommendations

Based on the analysis, the following recommendations are suggested to reduce cancellations and improve revenue:

| Key Finding | Recommendation | Objective |
| :--- | :--- | :--- |
| [cite_start]**High Cancellation Rate with Higher ADR** [cite: 530, 533] | [cite_start]**Implement dynamic and targeted pricing strategies**[cite: 534]. [cite_start]Offer location-based rate reductions and timely discounts to address price sensitivity[cite: 534]. | Reduce cancellations driven by high accommodation costs. |
| [cite_start]**January Cancellation Peak** [cite: 480, 535] | [cite_start]**Launch targeted marketing campaigns and special promotions in January**[cite: 536, 537]. This can help fill vacant rooms and offset the highest cancellation losses. | Stabilize revenue during the period of highest risk. |
| [cite_start]**Higher Cancellations in Resort Hotels** [cite: 538] | [cite_start]**Offer reasonable discounts on room prices during weekends or holidays** for Resort Hotels[cite: 539]. [cite_start]Resort rates naturally increase during these times, which correlates with higher cancellations[cite: 465, 538]. | Improve occupancy and reduce seasonal cancellations. |
| [cite_start]**Portugal (PRT) is the Top Cancellation Country** [cite: 526] | [cite_start]**Enhance overall hotel quality and service standards**, with a specific focus on understanding and addressing Portuguese customer feedback and booking behavior[cite: 541, 542]. | Mitigate cancellations from a key market segment. |

---
