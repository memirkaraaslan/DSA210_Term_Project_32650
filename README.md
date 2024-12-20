# DSA210_Term_Project__Sleep_Quality
The Relation Between My Daily Activities, Health Information, and My Sleep Quality

# Daily Activities and Sleep Quality Analysis

## Overview
This project explores the relationship between my daily activities and my sleep quality. By analyzing factors such as dietary intake, caffeine consumption, exercise routines, and meal timings, I aim to uncover patterns and insights to improve my sleep quality and overall well-being.

---

## Motivation
Sleep is a critical component of physical and mental health. Understanding how my daily choices—such as nutrition, caffeine intake, and exercise—affect my sleep quality can help me make informed decisions for a healthier lifestyle. This project provides a hands-on opportunity to apply data science techniques to real-life data and serves as a foundation for future data science applications and real-world health analytics.

---

## Data Collection
Data is collected daily from a combination of manual tracking and Galaxy Watch measurements. Key parameters include:

### **Daily Activity Parameters**
- **Nutritional Intake**: Total calories intake, carbohydrates, proteins, and fats (in grams).
    - The nutritional intake is measured using the app "FatSecret" to calculate the correspondent calories of foods.
- **Caffeine Consumption**: Total intake (in milligrams).
    - The caffeine content of beverages is recorded based on information from the product packaging or reliable online databases, such as the USDA FoodData Central or other trusted nutrition websites.
- **Hydration**: Water consumption (in liters).
- **Exercise**:
    - Presence (yes / no) and duration (in minutes)
    - Type i.e. exercise intensity (e.g., cardio, strength).
- **Meal Timings**: Breakfast, lunch, and dinner times.
- **Screen Time**:
    - Total phone screen usage (in hours).
    - Total time spent with computer games (in hours).
- **Mood**: Self-rated dominant mood (e.g., Happy, Tired, Stressed).
- **Stress Level**: Average stress level (scale of 1-10), measured using Galaxy Watch.
- **Steps**: Total steps taken during the day.
- **Mental Motivation**: Self-assessed motivation level (scale of 1-10).
- **Work/Study Time**: Time spent on work, education, or study activities (in hours).
- **Social Time**: Time spent socializing, including activities such as meeting with friends, participating in extracurricular activities (e.g., student clubs), and spending quality time with family.
- **Sleep and Wake Times**: Daily sleep and wake-up times.
- Additional Parameters for Better Insights:
    - Weather conditions: Daily weather condition data collected from "The Weather Channel" and manual tracking.
        - Temperature: Average air temperature during the day measured in degrees Celsius (°C).
        - Humidity: Recorded as a percentage (%).
        - Weather Conditions: Described as sunny, rainy, cloudy, etc.
    - Body composition information: The information collected daily regarding body composition and ratios between;
        - Mass (kg) information for: Body (measured with a scale) , Skeletal muscle, Fat, Body water
        - Body analysis: Body fat percentage, BMI (Body Mass Index) calculated using mass informations

### **Sleep Quality Parameters**
Collected via Galaxy Watch:
- **Sleep Stages**:
  - Awake time (minutes)
  - Light sleep (minutes)
  - REM sleep (minutes)
  - Deep sleep (minutes)
- **Oxygen Levels**:
  - Minimum blood oxygen percentage during sleep
- **Skin Temperature**:
  - Highest and lowest skin temperature during sleep
- **Heart Rate**:
  - Average, minimum, and maximum heart rates during sleep
- **Snoring Data**:
  - Presence (yes/no) and duration (if applicable).
  - Detected by the "Samsung Health" application installed on my smartphone.
- **Sleep Durations**:
  - Total sleep time (hours)
  - Sleep efficiency: Duration of actual sleep compared to total bed time
- **Device-Indicated Scores**:
  - Physical Recovery Rate
  - Rest Rate
  - Mental Recovery Rate
  - Number of Sleep Cycles
  - Total Sleep Score assessed by "Samsung Health"

**Planned Tools for Data Logging**:
- Manual input into a spreadsheet application (e.g., Excel or Google Sheets).
- Galaxy Watch for biometric and sleep quality measurements.
- Potential Future Integration with APIs or Apps.

**Note**: Data collection will begin shortly and is planned for a duration of 2-3 weeks.

---

## Analysis Plan
1. **Exploratory Data Analysis (EDA)**:
   - Identify trends in sleep quality with respect to different variables.
   - Visualize the data using scatter plots, bar charts, and heatmaps.

2. **Feature Engineering**:
   - Derive new features, such as total caloric intake or caffeine-to-sleep ratios.
   - Normalize and preprocess the data for modeling.
  
3. **Visualization**:
   - Create dashboards to illustrate findings and patterns clearly.
  
---

## Tools and Libraries
The following tools and libraries will be utilized throughout the project as the coding and analysis phase progresses:
- **Python**: pandas, numpy, matplotlib, seaborn
- **Jupyter Notebook**: For data exploration and analysis
- **GitHub**: For version control and project collaboration
- **Spreadsheet Software**: Excel or Google Sheets for data collection

This README will be updated regularly as the project progresses.

---

## Sample Data
### Sample Data: Daily Activity
| Date       | Total Calories | Carbs (g) | Protein (g) | Fat (g) | Caffeine (mg) | Hydration (L) | Breakfast Time | Lunch Time | Dinner Time | Screen Time (hrs) | Gaming Time (hrs) | Mood       | Stress Level (1-10) | Steps  | Mental Motivation (1-10) | Work/Study Time (hrs) | Social Time (hrs) | Sleep Time | Wake Time |
|------------|----------------|-----------|-------------|---------|---------------|---------------|----------------|------------|-------------|-------------------|--------------------|------------|---------------------|--------|---------------------------|-----------------------|-------------------|-----------|-----------|
| 2024-01-01 | 2000           | 200       | 80          | 60      | 150           | 2.0           | 08:00          | 13:00      | 19:00       | 4.0               | 1.5                | Happy      | 3                   | 8000   | 9                         | 5.0                   | 2.0               | 23:00     | 07:00     |
| 2024-01-02 | 1800           | 180       | 90          | 50      | 120           | 1.8           | 08:15          | 13:15      | 19:30       | 5.0               | 2.0                | Stressed   | 5                   | 10000  | 7                         | 4.5                   | 1.5               | 23:30     | 06:30     |
| 2024-01-03 | 2500           | 250       | 100         | 70      | 200           | 2.5           | 07:45          | 12:45      | 18:45       | 3.0               | 1.0                | Relaxed    | 2                   | 12000  | 10                        | 6.0                   | 2.5               | 22:30     | 06:00     |

---

### Sample Data: Additional Parameters
| Date       | Air Temperature (°C) | Humidity (%) | Weather Condition | Body Weight (kg) | Skeletal Muscle (kg) | Body Fat (%) | Body Water (%) | BMI  |
|------------|-----------------------|--------------|-------------------|------------------|----------------------|--------------|----------------|------|
| 2024-01-01 | 25.0                  | 60           | Sunny             | 70.0             | 30.0                 | 18.0         | 55.0           | 24.5 |
| 2024-01-02 | 22.0                  | 55           | Cloudy            | 69.5             | 29.8                 | 17.5         | 54.5           | 24.3 |
| 2024-01-03 | 20.0                  | 65           | Rainy             | 71.0             | 31.0                 | 19.0         | 56.0           | 25.1 |

---

### Sample Data: Sleep Quality Parameters
| Date       | Sleep Time | Wake Time | Total Sleep Time (hrs) | REM Sleep (min) | Light Sleep (min) | Deep Sleep (min) | Awake Time (min) | Min O2 (%) | Max Skin Temp (°C) | Min Skin Temp (°C) | Avg Heart Rate (bpm) | Min Heart Rate (bpm) | Max Heart Rate (bpm) | Snoring (mins) | Physical Recovery (%) | Rest Rate (%) | Mental Recovery (%) | Number of Sleep Cycles | Total Sleep Score | Sleep Efficiency (%) |
|------------|------------|-----------|-------------------------|-----------------|-------------------|------------------|------------------|------------|---------------------|---------------------|-----------------------|-----------------------|-----------------------|----------------|------------------------|--------------|----------------------|-------------------------|-------------------|-----------------------|
| 2024-01-01 | 23:00      | 07:00     | 8.0                     | 90              | 250               | 60               | 20               | 95         | 35.0                | 33.0                | 60                    | 50                    | 70                    | 0              | 85                     | 80           | 90                   | 5                       | 88                | 90                    |
| 2024-01-02 | 23:30      | 06:30     | 7.0                     | 85              | 260               | 50               | 25               | 93         | 34.5                | 32.5                | 65                    | 55                    | 75                    | 5              | 80                     | 75           | 85                   | 4                       | 82                | 85                    |
| 2024-01-03 | 22:30      | 06:00     | 7.5                     | 100             | 230               | 70               | 15               | 96         | 36.0                | 34.0                | 62                    | 52                    | 72                    | 2              | 88                     | 85           | 92                   | 6                       | 90                | 87                    |


---

## Findings
The insights derived from this project are expected to include:
- The impact of dietary habits (e.g., high-carb vs. high-protein meals) on specific sleep stages such as REM or deep sleep.
- The effect of caffeine consumption on sleep duration, quality, and recovery rates (physical, mental, and restfulness scores).
- The relationship between hydration levels and biometric sleep parameters such as heart rate, blood oxygen levels, and skin temperature.
- Correlations between exercise routines (e.g., intensity, duration) and sleep improvement, particularly in physical recovery metrics.
- How external factors like screen time, stress levels, and mood influence sleep stages and overall restfulness.
- Patterns observed in sleep cycles (e.g., how consistent wake-up and bedtimes contribute to better sleep quality).
- Insights into the role of environmental factors such as weather conditions on sleep efficiency.
- An overall understanding of what combinations of daily activities (e.g., exercise, meal timings, and mental motivation) promote the best sleep outcomes.

---

## Limitations and Future Work
### Limitations:
- **Self-Reported Data**: Daily activity logs (e.g., nutrition, screen time, stress) are manually recorded and may contain biases or inaccuracies.
- **Device Accuracy**: While Galaxy Watch provides detailed sleep and biometric data, its measurements are limited by the precision and reliability of the device.
- **Individual Scope**: The analysis is limited to my personal lifestyle and may not generalize to a wider population.
- **Short Observation Period**: The dataset may not cover a sufficient time period to identify long-term patterns and trends.

### Possible Improvements:
- **Enhanced Data Collection**:
  - Develop or use an automated logging system that integrates wearable device data with external APIs (e.g., weather or stress tracking apps).
  - Incorporate additional metrics such as daily caloric intake or detailed exercise intensity levels using fitness trackers.
- **Longer Study Period**: Extend the data collection over several months or even a year to observe seasonal and long-term trends.
- **Comparative Analysis**: Compare my data with anonymized datasets from other individuals to identify broader patterns and validate findings.
- **Advanced Modeling Techniques**:
  - Utilize time-series analysis to predict sleep quality based on historical data.
  - Apply clustering techniques to categorize "high-quality sleep days" vs. "low-quality sleep days" and analyze contributing factors.
- **Visualization and Dashboards**:
  - Create an interactive dashboard to visualize relationships between variables and allow for scenario testing (e.g., "How does skipping caffeine impact sleep quality?").
- **Environmental Data**:
  - Integrate weather API data (temperature, humidity, air quality) to explore correlations with sleep metrics like deep sleep duration or physical recovery.
- **Public Sharing**:
  - Share findings through a user-friendly web application or generalizable sleep-quality improvement framework.
  - Publish a report or blog post summarizing the key insights and actionable recommendations for others.

---

## Repository Structure in Progress
```plaintext
|-- data/
|   |-- daily_logs.csv         # Collected data (processed)
|-- notebooks/
|   |-- eda.ipynb              # Exploratory Data Analysis
|   |-- analysis.ipynb         # Data Analysis and Visualization
|-- README.md                  # Project overview and details
|-- requirements.txt           # Python dependencies
