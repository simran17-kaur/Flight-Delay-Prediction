# ✈️ Flight Delay Prediction using Deep Learning  

> Predicting commercial flight delays using flight records, weather, and airport data.  

---

## 🔎 Overview  
Flight delays are a persistent challenge in the aviation industry, affecting passengers, airlines, and operations.  
This project leverages **Deep Learning** and **Data Science** techniques to analyze **2023 U.S. Civil Flight data** enriched with **weather and geolocation features**, aiming to predict delays with higher accuracy.  

By combining operational, environmental, and spatial datasets, this project demonstrates how **data-driven insights** can help airlines and airports improve scheduling efficiency and reduce disruptions.  

---

## 🎯 Objectives  
1. Perform exploratory data analysis (EDA) on flight, weather, and airport datasets.  
2. Identify operational hotspots (airlines/airports with frequent delays).  
3. Engineer predictive features: departure time, route, weather conditions, airline performance.  
4. Train deep learning models for binary/multi-class classification of delays.  
5. Evaluate model performance and visualize delay patterns.  

---

## 📊 Datasets  
Source: [2023 US Civil Flights: Delay, Meteo & Aircraft (Kaggle)](https://www.kaggle.com/datasets/bordanova/2023-us-civil-flights-delay-meteo-and-aircraft?select=US_flights_2023.csv)  

- **maj_us_flight_Jan2024.csv** – major U.S. flights with timings, delays, and aircraft details.  
- **weather_meteo_by_airport.csv** – weather conditions at airports (wind, temperature, precipitation).  
- **airports_geolocation.csv** – latitude/longitude and spatial details of airports.  
- **Cancelled_Diverted_2023.csv** – records of cancelled/diverted flights.  

**Key Features**  
- Flight schedule: departure/arrival times, route, airline.  
- Delay metrics: departure delay, arrival delay.  
- Weather: wind, precipitation, temperature.  
- Airport info: traffic volume, location.  

---
### 🔧 Exploratory Data Analysis  
- Visualized **delay patterns** (departure vs arrival).  
- Analyzed **airline-wise and airport-wise performance**.  
- Correlated **weather factors** with delays.  
- Identified outliers (early departures, extreme delays).

## 📈 Insights from EDA  
- Evening flights tend to face higher delays.  
- Weather factors (wind speed, precipitation) significantly affect punctuality.  
- Airlines vary in performance — some consistently manage on-time schedules better.  

---

## 🛠 Methods & Models  

### 1️⃣ Feedforward Neural Network (FFNN)  
- **Input:** flight + weather features.  
- **Architecture:** Dense layers with dropout.  
- **Optimizer:** Adam, Loss = Binary Crossentropy.  
- **Purpose:** Establish baseline predictive performance.  

### 2️⃣ Deep & Wide Neural Network (DWNN)  
- **Wide component:** Linear (shallow) model to capture direct feature interactions.  
- **Deep component:** Dense hidden layers for high-level abstractions.  
- **Combined output:** Concatenation of deep + wide layers, passed through softmax.  
- **Purpose:** Handle both memorization (wide) and generalization (deep). 

---


