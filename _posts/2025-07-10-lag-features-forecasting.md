---
title: "My Forecast Was Wrong — Until I Added Lag Features"
date: 2025-07-10
author: Aarti Kumari
categories: [Time Series, Forecasting]
tags: [lag features, machine learning, forecasting, sales, rolling average]
permalink: /lag-features-forecasting/
read_time: true
---

When I first started building a sales forecasting model, I focused heavily on choosing the “best” machine learning algorithm — Linear Regression, Random Forest, XGBoost… you name it.

But no matter how many models I tried, the forecasts felt off — too smooth, too delayed, or just wrong.

That’s when I learned something that completely shifted my approach:

> **In time-based forecasting, what you feed the model matters more than which model you use.**

And that’s where **lag features** come in.

---

## 🚨 The Problem

> “I initially built a model using only time as input. The predictions were smooth, but totally disconnected from the real trend. That’s when I realized: the model had no memory of the past.”

---

## ✅ The Fix: Adding Lag Features

Lag features are values from the past that we bring into the current row.

Here’s what I added:

- `Sales_Lag_1`: Sales from 1 week ago  
- `Sales_Lag_2`: Sales from 2 weeks ago  
- `Sales_Lag_12`: Sales from the same week last quarter  
- `Rolling_Mean_4`: 4-week rolling average  
- `Rolling_Std_4`: 4-week rolling standard deviation  

> “I added lag features like `lag_1` and a `rolling_mean_12`. Suddenly, the model started making smarter predictions.”

---

## 🔬 Case Study: Forecasting Sunspots

**Dataset Used:**  
I used the publicly available *Monthly Sunspots* dataset — clean and ready to use.

👉 _[Download here](https://www.kaggle.com/datasets/robervalt/sunspots)_

---

### 📊 Model Comparison

| Model | Description | MAE (Error) |
|-------|-------------|-------------|
| No Lag Features | Used only time index | 60.28 |
| With Lag Features | Used lag_1 + rolling_mean_12 | **13.65** |

![image](https://github.com/user-attachments/assets/7b9fe1c9-7c0a-47ec-a7a1-b1450b59aecc)

✅ **Result**: Error reduced significantly by giving the model memory.

---

## 📈 Visual Comparison

![image](https://github.com/user-attachments/assets/38f0134d-9ad2-47b9-b22f-2c4e433c3179)


---

## 🧠 Final Takeaway

Adding memory to your model through **lag** and **rolling** features can be the difference between guessing and forecasting.

---

👉 **[Get Full Code Here](https://www.kaggle.com/code/aarti16/sunspot)**  

