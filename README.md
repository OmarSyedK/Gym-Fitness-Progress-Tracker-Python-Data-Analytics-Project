# Gym & Fitness Progress Tracker

A Python-based fitness analytics project that transforms 90 days of workout data into meaningful insights using **Pandas**, **NumPy**, and **Matplotlib**.

## Project Overview

Fitness tracking is an essential part of maintaining a healthy lifestyle, yet many individuals still rely on notebooks or spreadsheets to record their progress. These methods make it difficult to identify trends, evaluate performance, or measure long-term improvement.

The **Gym & Fitness Progress Tracker** addresses this challenge by analyzing workout records over a 90-day period. It cleans raw fitness data, performs weekly and monthly analyses, tracks body weight changes, and visualizes workout patterns to provide actionable insights for gym members and personal trainers.

---

## Project Objectives

- Load and analyze daily workout records from a CSV file.
- Clean missing and inconsistent workout data.
- Track body weight changes over 90 days.
- Analyze calories burned and workout durations.
- Identify the most and least active weeks.
- Generate weekly and monthly fitness summaries.
- Visualize workout trends using charts.

---

## Dataset Description

The project uses a dataset containing **90 days of workout records**.

| Column | Description |
|---------|-------------|
| Date | Workout date |
| Workout_Type | Cardio, Strength, Flexibility, Sports, Rest Day |
| Duration_Minutes | Workout duration in minutes |
| Calories_Burned | Calories burned during the workout |
| Body_Weight_KG | Daily body weight in kilograms |
| Reps_or_Sets | Sets, repetitions, or workout details |
| Notes | Additional workout notes |

The dataset intentionally includes:

- Missing workout records
- Negative workout durations
- Unrealistic calorie values
- Incorrect body weight entries

These issues were cleaned during preprocessing to simulate real-world data quality challenges.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

---

## Project Workflow

### Step 1 – Data Creation

- Created a realistic 90-day workout dataset.

### Step 2 – Data Exploration

- Loaded the dataset using `pandas.read_csv()`
- Explored the data using:
  - `head()`
  - `info()`
  - `describe()`

### Step 3 – Data Cleaning

- Converted dates to datetime format.
- Filled missing workout records.
- Corrected negative workout durations.
- Replaced unrealistic calorie values.
- Corrected invalid body weight entries.

### Step 4 – Weekly Analysis

- Grouped workout records by week.
- Calculated:
  - Weekly average workout duration
  - Weekly calories burned
  - Total workouts completed

### Step 5 – Weight Trend Analysis

- Used NumPy to calculate:
  - Starting weight
  - Ending weight
  - Average weight
  - Weight change
- Created a line chart showing weight trends.

### Step 6 – Workout Distribution

- Counted workout types using `value_counts()`.
- Created a bar chart showing workout frequency.

### Step 7 – Performance Insights

Generated key metrics including:

- Best performing week
- Least active week
- Most calories burned in a day
- Average workout duration
- Total calories burned

### Step 8 – Monthly Summary

Grouped records by month to calculate:

- Total workouts
- Total calories burned
- Average body weight

---

## Visualizations

The project includes the following visualizations:

- Line chart showing body weight changes over 90 days.
- Bar chart displaying workout frequency by workout type.

---

## Key Insights

- Body weight showed an overall downward trend across the 90-day period.
- Weekly analysis identified the most and least active training weeks.
- Monthly summaries highlighted changes in workout intensity.
- Strength and Cardio were among the most frequently performed workouts.
- Data cleaning significantly improved the quality and reliability of the analysis.
- Performance metrics provided measurable evidence of fitness progress.

---

## Project Structure

```text
Gym-Fitness-Progress-Tracker/
│
├── Gym_Fitness_Progress_Tracker.ipynb
├── fitness_workout_log.csv
├── images/
│   ├── weight_trend.png
│   └── workout_distribution.png
└── README.md
```

---

## How to Run

1. Clone this repository.

```bash
git clone https://github.com/<your-username>/Gym-Fitness-Progress-Tracker.git
```

2. Navigate to the project directory.

```bash
cd Gym-Fitness-Progress-Tracker
```

3. Install the required libraries.

```bash
pip install pandas numpy matplotlib
```

4. Open the Jupyter Notebook or Google Colab notebook.

5. Run all cells sequentially.

---

## Future Improvements

- Develop an interactive dashboard using Streamlit or Plotly.
- Include BMI and Body Fat Percentage analysis.
- Add personalized workout recommendations.
- Implement goal tracking and progress notifications.
- Generate automated PDF reports.

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Time-series analysis
- Data aggregation using Pandas
- Statistical analysis using NumPy
- Data visualization using Matplotlib
- Transforming raw fitness data into meaningful insights

---



