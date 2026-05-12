# Flight-Delay-Prediction

![Airplane Wing](https://images.unsplash.com/photo-1436491865332-7a61a109cc05?q=80&w=2074&auto=format&fit=crop)

## Introduction
Delay is one of the most remembered performance indicators of any transportation system. Notably, commercial aviation players understand delay as the period by which a flight is late or postponed. Thus, a delay may be represented by the difference between scheduled and real times of departure or arrival of a plane. Indeed, flight delay is an essential subject in the context of air transportation systems. 

To better understand the entire flight ecosystems, vast volumes of data from commercial aviation are collected every moment and stored in databases. Submerged in this massive amount of data, data scientists extract useful information to solve challenging logistical problems. In this project, we've performed an extensive data analysis to extract the important attributes/factors responsible for flight delays. By synthesizing historical flight schedules with real-time meteorological conditions and air traffic telemetry, this predictive analytics dashboard empowers aviation stakeholders to transition from reactive crisis management to proactive logistical planning.

## Problem Statement
Flight delays are quite frequent and are a major source of frustration and cost for passengers and airlines alike (costing the global industry over $30 Billion annually). As we will see, some flights are more frequently delayed than others, and there is high interest in providing this information to travelers.

Flight prediction is crucial during the decision-making process for all players in commercial aviation. However, the development of accurate prediction models for flight delays has become cumbersome due to the complexity of the air transportation system and the deluge of flight data. Traditional frameworks rely on static timetables and fail to dynamically adjust to real-time environmental volatility or the systemic "Ripple Effect." Based on the data, we aim to analyze the major causes of flight delays and assign a probability on whether a particular flight will be delayed.

## Objective
The objective of the project is to perform analysis of historic flight data to gain valuable insights and build a predictive model to predict whether a flight will be delayed or not given a set of flight characteristics. 

**Questions to be answered post-analysis:**
* Does the month or day of the week have any impact on flight delays?
* Flights to which destination have seen the most delays?
* Which time of day is most suitable for preventing flight delays?
* Which airline has the highest number of flights delayed?
* What are the primary causes for flight delays (e.g., Weather, NAS bottlenecks, Late Aircraft Arrival)?

The primary objective of the predictive model is to forecast domestic flight delays with >90% accuracy utilizing advanced spatio-temporal data and machine learning algorithms (XGBoost, Random Forest, CatBoost, LSTM). Such a model will help both passengers and airline companies predict future delays and minimize them.

## Dataset Details
**Datasets obtained and integrated from:**
* **Bureau of Transportation Statistics (BTS):** 7.2 Million US domestic flight performance records (2023-2024).
* **Real-Time Telemetry APIs:** OpenWeatherMap API (visibility, wind, precipitation) and FlightRadar24 / ADS-B feeds for real-time air traffic metrics.

## Project Design
This project strictly follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) framework.

*(Below is the structural representation of our Machine Learning pipeline)*
<img width="1122" height="1402" alt="FLight delay prediction ML Pipeline" src="https://github.com/user-attachments/assets/ce97f266-8281-4981-9833-effd48c81750" />

![Project Design Flowchart](https://via.placeholder.com/850x350.png?text=https://kommodo.ai/i/1SXIO5UHZD1LokGxYdPM)

* **Data Ingestion:** Importing and merging historical CSVs with live APIs.
* **Pre-processing & Cleaning:** Handling missing values, one-hot encoding, and applying **SMOTE** to balance the dataset.
* **Data Visualization:** Identifying trends and temporal delay peaks.
* **Modelling:** Training models (XGBoost, CatBoost, Random Forest).
* **Prediction:** Outputting delay probability via a user-friendly Web Dashboard.

## 💻 Technologies Used
* **Machine Learning (Backend Logic):** Python, XGBoost, CatBoost, Random Forest, LSTM (Deep Learning), SMOTE, LIME.
* **Data Processing:** Pandas, NumPy, Scikit-learn.
* **Frontend Dashboard:** HTML5, CSS3, Vanilla JavaScript.
* **Deployment:** GitHub Pages (Interactive UI hosting).

## 🚀 Steps to Get Started
To view and interact with the flight prediction dashboard locally on your machine:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/](https://github.com/)[your-github-username]/flight-delay-dashboard.git
    ```
2.  **Navigate to the Directory:**
    ```bash
    cd flight-delay-dashboard
    ```
3.  **Run the Application:**
    Since the dashboard is built with pure HTML/CSS/JS, no server installation is required. Simply double-click the `index.html` file to open it in your default web browser.
4.  **Live Demo:** Alternatively, you can view the live deployed dashboard here: [Insert Your GitHub Pages Link Here]

---
*This repository contains the front-end simulation and documentation for the MBA Aviation Analytics capstone project.*
