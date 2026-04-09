# 🏠 Neighborhood Air Quality & Housing Value
**HOML Chapter 2 - End-to-End Project**

## 🎯 The Goal
Predicting housing prices while accounting for local air quality to understand environmental impact on property value.

## 🚧 Challenges & Conquests
*List the problems you hit while practicing Chapter 2 here.*

### 1. The "Bad Data" Hurdle
- **The Problem:** The Air Quality dataset had weird placeholders like `-200` instead of missing values.
- **The Conquest:** I used `df.replace()` to turn them into `NaN` so my Scikit-Learn `SimpleImputer` could actually see them.

### 2. The "Category" Confusion
- **The Problem:** `OneHotEncoder` created way too many columns for the 'Neighborhood' feature.
- **The Conquest:** I learned about "Feature Engineering" and grouped smaller neighborhoods together to keep the model simple.

## 🛠️ Recommendations for Future Me
- Try using **Polynomial Features** to see if the relationship between pollution and price isn't just a straight line.
- Automate the whole thing using a **Scikit-Learn Pipeline**.
