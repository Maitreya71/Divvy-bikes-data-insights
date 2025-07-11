## 🚴‍♂️ Divvy Bike Sharing – Exploratory Data Analysis & Power BI Dashboard

### 📌 Project Overview

This project showcases **Exploratory Data Analysis (EDA)** performed using Python on Divvy bike-sharing trip data, followed by the creation of a **Power BI dashboard** to visualize usage patterns, rider behavior, and trip trends. The analysis supports better understanding of commuter vs casual usage and identifies seasonal or operational insights.

### 📂 Dataset Description

* **Source**: divvy bike data in the link - (https://drive.google.com/drive/folders/1VA5Xf4QMeiPwQhQ7a9-tfw6PD5eVsBFw?usp=drive_link)
* **Format**: CSV
* **Timeframe**: four full calendar years from 2018-2021
* **Key Fields**:

  * `ride_id`, `rideable_type`
  * `started_at`, `ended_at`
  * `start_station_name`, `end_station_name`
  * `member_casual` (rider type)
  * Time features: day of week, month, hour
  * Trip duration (calculated)



### 🧪 Exploratory Data Analysis (Python)

Performed using the attached Jupyter Notebook: **`Analyzing_divvy_tripdata.ipynb`** and **trips-4yr.ipynb**

#### ✅ Analysis Highlights:

* Converted timestamps (`started_at`, `ended_at`) to `datetime`
* Calculated **trip durations** and filtered outliers (e.g., negative or excessively long trips)
* Extracted **weekday, month, hour** from datetime for time-based patterns
* Grouped and visualized data by:

  * **Rider type** (member vs casual)
  * **Bike type** (electric, docked, classic)
  * **Trip duration** statistics
  * **Monthly and weekly usage** trends
* Visualizations created using **Seaborn** and **Matplotlib**



### 📊 Power BI Dashboard

An interactive dashboard was created using **Power BI Desktop** to complement the Python analysis.

#### 📈 Dashboard Features:

* **Rider Type Breakdown**: Trip counts, average durations, and bike preferences
* **Time Trends**: Monthly and weekday usage patterns
* **Station Analysis**: top Busy stations
* **Trip Duration**: Distribution by rider type and weekday
* **Interactive Filters**: By rider type, month, bike type

---

### 📁 Repository Structure

```
divvy-bike-analysis/
├── data/
│   └── zip folder containing csv files            # source data of csv files in folder
├── notebooks/
│   └── Analyzing_divvy_tripdata.ipynb
    └── trips-4yr.ipynb
├── dashboard/
│   └── divvy_dashboard.pdf                       #pdf version of .pbix dashboard format 
├── README.md
```



### 📌 How to Run

1. Clone the repository
2. Open and run `Analyzing_divvy_tripdata.ipynb` and `trips-4yr.ipynb` in Jupyter notbook to view EDA
3. Open `divvy_dashboard.pbix` in Power BI Desktop to explore visual insights


### 🧠 Key Insights

* Casual riders take longer trips, mostly on weekends
* Members prefer weekday commutes and shorter rides
* Summer months show peak usage, especially among casual users
* Electric bikes are increasingly popular among casual riders


### 🚀 Future Work

* Add weather integration for ride behavior analysis
* Use clustering for station demand prediction
* Deploy dashboard to Power BI Service with auto-refresh
