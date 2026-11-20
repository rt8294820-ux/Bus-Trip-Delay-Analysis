# 🚌 Bus Trip Delays Analysis

## 📌 Project Overview

This project analyzes a public transportation dataset containing bus trip schedules, actual arrival/departure times, weather conditions, traffic levels, passenger counts, and route information. The goal is to identify patterns and factors contributing to bus delays and generate actionable insights using Python-based data analysis techniques.

## 🎯 Objectives

- Clean and preprocess raw transportation data.
- Calculate arrival and departure delays.
- Identify delayed versus on-time trips.
- Analyze delays across different routes.
- Examine the impact of traffic conditions and weather on punctuality.
- Study delay trends by day of the week and time of day.
- Generate summary statistics for operational performance evaluation.

## 📂 Dataset Description

The dataset contains bus trip records with the following attributes:

| Column | Description |
|----------|------------|
| trip_id | Unique trip identifier |
| date | Date of trip |
| day_of_week | Day on which the trip occurred |
| route | Bus route identifier |
| bus_id | Unique bus identifier |
| origin | Starting location |
| destination | Ending location |
| scheduled_departure | Planned departure time |
| actual_departure | Actual departure time |
| scheduled_arrival | Planned arrival time |
| actual_arrival | Actual arrival time |
| weather | Weather conditions during the trip |
| traffic_level | Traffic congestion level |
| passenger_count | Number of passengers |

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## 🔄 Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Inspected dataset structure and summary statistics.
3. Checked for missing values and duplicate records.
4. Removed duplicate entries.
5. Removed rows containing missing values.
6. Converted date and time columns into datetime format.
7. Calculated arrival and departure delays in minutes.

## 📊 Analysis Performed

### Delay Calculation
- Arrival Delay = Actual Arrival − Scheduled Arrival
- Departure Delay = Actual Departure − Scheduled Departure

### Delay Classification
Trips were classified into:
- **Delayed**: Arrival delay greater than 0 minutes
- **On Time or Early**: Arrival delay less than or equal to 0 minutes

### Key Performance Metrics
- Total number of trips
- Number of delayed trips
- Average delay time
- Maximum delay recorded
- Delay percentage

### Route-Based Analysis
Average delay was calculated for each route to identify routes with higher delay frequencies.

### Time-Based Analysis
Trips were grouped into:
- Morning (00:00–11:59)
- Afternoon (12:00–16:59)
- Evening (17:00–23:59)

Average delays were analyzed for each period.

### Day-of-Week Analysis
Delay trends were compared across all days of the week to identify recurring congestion patterns.

### Traffic Impact Analysis
Average delay was analyzed across:
- Low Traffic
- Medium Traffic
- High Traffic

### Weather Impact Analysis
Average delay was examined under different weather conditions such as:
- Clear
- Cloudy
- Rainy

## 📈 Expected Insights

This analysis helps answer questions such as:

- Which routes experience the most delays?
- How does weather affect bus punctuality?
- Does heavy traffic significantly increase delays?
- Which days have the highest average delays?
- What time of day is most prone to delays?

## ▶️ Running the Project

1. Clone this repository:

```bash
git clone https://github.com/your-username/bus-trip-delays-analysis.git
```

2. Install required libraries:

```bash
pip install pandas numpy matplotlib
```

3. Place the dataset file (`bus_trip_delays_dataset.csv`) in the project directory.

4. Run the Python script:

```bash
python capstone_project_1.py
```

## 📁 Project Structure

```text
├── capstone_project_1.py
├── bus_trip_delays_dataset.csv
└── README.md
```

## 🚀 Future Improvements

- Interactive dashboards using Power BI or Tableau.
- Delay prediction using Machine Learning models.
- Route optimization recommendations.
- Real-time delay monitoring and visualization.

## 👨‍💻 Author

**Shaurya Thapa**

Data Analysis Capstone Project focused on public transportation performance and delay analysis.
