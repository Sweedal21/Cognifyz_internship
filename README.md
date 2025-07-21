# 🍽️ Restaurant Dataset Analysis

This project involves a detailed analysis of restaurant data to derive insights about services, geolocation, cuisines, customer ratings, and more. The dataset includes information on 9551 restaurants across various countries, with features such as location, services offered, ratings, and pricing.

---

## 📁 Dataset Columns

| Column Name             | Description |
|-------------------------|-------------|
| `Restaurant ID`         | Unique identifier for each restaurant |
| `Restaurant Name`       | Name of the restaurant |
| `Country Code`          | Country reference code |
| `City`                  | City where the restaurant is located |
| `Address`               | Full address of the restaurant |
| `Locality`              | Neighborhood/local region |
| `Locality Verbose`      | Extended locality details |
| `Longitude`             | Longitude coordinate |
| `Latitude`              | Latitude coordinate |
| `Cuisines`              | Types of cuisines offered |
| `Average Cost for two`  | Average cost for two people |
| `Currency`              | Currency used in pricing |
| `Has Table booking`     | Indicates if table booking is available |
| `Has Online delivery`   | Indicates if online delivery is available |
| `Is delivering now`     | Shows real-time delivery availability |
| `Switch to order menu`  | Navigation option for ordering |
| `Price range`           | Cost range from 1 (low) to 4 (high) |
| `Aggregate rating`      | Average customer rating |
| `Rating color`          | Color code for rating |
| `Rating text`           | Text description of the rating |
| `Votes`                 | Number of user votes/ratings |

---

## 🧪 Data Exploration and Preprocessing

- **Shape of Data:** 9551 rows × 21 columns
- **Missing Values:**  
  - Only the `Cuisines` column has missing values (9 nulls), handled via:
    - Imputation with mode or
    - Dropping if required
- **Data Type Check:** Ensured correct data types for numerical and categorical fields.
- **Target Variable - `Aggregate rating`:**  
  - Distribution analyzed to check class imbalance  
  - Most ratings are clustered around 3.0–4.5

---

## 📊 Descriptive Analysis

- **Numerical Stats:**  
  - Calculated **mean, median, std, min, max** for:  
    - `Votes`, `Average Cost for two`, `Aggregate rating`
- **Categorical Distribution:**  
  - Explored frequency counts for:
    - `Country Code`, `City`, and `Cuisines`
- **Top Categories Identified:**
  - Most common **cities** and **cuisines**
  - Most frequent restaurant names

---

## 🌍 Geospatial Analysis

- **Map Visualization:**
  - Used `Latitude` and `Longitude` to plot restaurants
- **Distribution Across Locations:**
  - Country-wise and city-wise count of restaurants
- **Correlation:**
  - Checked for any relationship between location and `Aggregate rating`

---

## 📅 Table Booking and Online Delivery

- **Service Availability:**
  - % of restaurants offering:
    - Table booking
    - Online delivery
- **Impact on Ratings:**
  - Compared average ratings:
    - With vs. without **table booking**
    - Online delivery availability across **price ranges**

---

## 💰 Price Range Analysis

- **Most Common Price Range:**  
  - Identified dominant price tier
- **Ratings by Price Range:**  
  - Analyzed average ratings for each price category
- **Rating Color Analysis:**
  - Mapped rating colors with price tiers to find the highest-rated category

---

## 🧠 Feature Engineering

- **Derived Features Created:**
  - `Restaurant Name Length`
  - `Address Length`
- **Binary Features Encoded:**
  - `Has Table Booking` → 1/0
  - `Has Online Delivery` → 1/0
  - `Is Delivering Now` → 1/0

---

## 🛠️ Tools & Libraries Used

- **Programming Language:** Python  
- **Key Libraries:**  
  - `pandas`, `numpy` → Data manipulation  
  - `matplotlib`, `seaborn`, `plotly`, `folium` → Visualization  
  - `sklearn` → Preprocessing  
  - `jupyter notebook` → Development environment  

---

## 📈 Insights & Outcomes

- High-rated restaurants commonly fall in mid to high price ranges.
- Online delivery and table booking positively influence ratings.
- Certain cuisines and cities dominate the dataset, impacting overall trends.

---

## 🚀 Future Work

- Build a model to **predict restaurant ratings**.
- Use **clustering** to identify food hotspots.
- Integrate **sentiment analysis** of reviews if available.

---

