# Gen-Z-Mental-Wellness-Analysis
This project explores the relationship between lifestyle habits, demographics, and mental health outcomes among Gen Z users. The goal is to uncover key drivers of anxiety and wellbeing and provide actionable insights for better decision-making in mental wellness strategies.


### TABLE OF CONTENT
* [Project Overview](#project-overview)
* [Dataset Overview](#dataset-overview)
* [Data Cleaning](#data-cleaning)
* [Tools](#tools)
* [Excel Dashboard](#excel-dashboard)
* [Dashboard](#dashboard)
* [Key Insights](#key-insights)
* [Interactive Analysis](#interactive-analysis)
* [Recommendation](#recommendation)
* [Data Source](#data-source)
* [Conclusion](#conclusion)


### PROJECT OVERVIEW
This project explores the relationship between lifestyle habits, demographics, and mental health outcomes among Gen Z users. The goal is to uncover key drivers of anxiety and wellbeing and provide actionable insights for better decision-making in mental wellness strategies.


### TOOLS
- SQL (PostgreSQL)
  > Data cleaning, transformation and querying
- Power BI
  > Data visualization and interactive dashboard creation
  

### DATASET OVERVIEW

COLUMNS:
- Age
- Gender
- Country
- Student_Working_Status
- Daily_Social_Media_Hours
- Screen_Time_Hours
- Night_Scrolling_Frequency
- Online_Gaming_Hours
- Content_Type_Preference
- Exercise_Frequency_per_Week
- Daily_Sleep_Hours
- Caffeine_Intake_Cups
- Study_Work_Hours_per_Day
- Overthinking_Score
- Anxiety_Score
- Mood_Stability_Score
- Social_Comparison_Index
- Sleep_Quality_Score
- Motivation_Level
- Emotional_Fatigue_Score
- Wellbeing_Index
- Burnout_Risk

DATASET SAMPLE PREVIEW:
|Age| Gender| Country | Student_Working_Status|Daily_Social_Media_Hours| Screen_Time_Hours| Night_Scrolling_Frequency|Online_Gaming_Hours| Content_Type_Preference|Exercise_Frequency_per_Week| Daily_Sleep_Hours|Caffeine_Intake_Cups|Study_Work_Hours_per_Day|Overthinking_Score|Anxiety_Score|Mood_Stability_Score|Social_Comparison_Index|Sleep_Quality_Score| Motivation_Level|Emotional_Fatigue_Score| Wellbeing_Index|Burnout_Risk|
|----|--------|-----|-------------------------|-------------------------|------------------|-------------------------|------------------|-------------------------|-----------------|----------------|-------------------|--------------------|-------------------------|------------------|-------------|-------------------|----------------|------------------|----------------|----------------|------------|
|24| Male| Canada |	Working | 4.81 |6.93 |	2.61 |	2.07 | News | 5.41 | 6.84 |	1.52 |11.42| 4.95|4.13|5.74|4.67|6.27|6.13|6.45|4.28|Medium|
|21| Male| USA | Student | 4.16|7.94 |	1.85 |	3.58 | Gaming | 3.41 | 7.88 |	2.23 |6.98| 5.91|3.63|5.75|5.38|7.37|6.27|3.74|5.23|Medium|
|25| Male| Pakistan | Student | 3.07|7.45|	2.96 |	2.85 | Entertainment | 3.4 | 6.39 |	0.53 |7.79| 4.06|5.67|6.03|2.41|6.48|4.82|6.69|3.72|High|
|25| Male| Pakistan | Student | 4.41|7.34|	4.51 |	3.37 | Educational | 2.19| 7.92 |	0.58 |6.61| 6.1|4.78|4.85|5.86|7.27|5.17|5.96|3.97|High|

### DATA CLEANING
- Changed date and amount datatype to date and currency format 
- Removed, duplicate, missing or invalid values


### DATA EXPLORATION 
1. Anxiety score by Gender
 ```SQL
SELECT u.gender,
ROUND(AVG(m.Anxiety_Score),2) AS Anxiety_score
FROM users u
JOIN mental_health m ON u.user_id = m.user_id
GROUP BY u.gender
ORDER BY Anxiety_score DESC;
```

2.Wellbeing index by sleep quality
```SQL
SELECT ROUND(AVG(m.sleep_quality_score),2) AS sleep_quality_Score,
RROUND(AVG(m.wellbeing_index),2) AS Wellbeing
FROM engagement_lifestyle e
JOIN mental_health m ON e.user_id = m.user_id
GROUP BY e.sleep_quality_Score 
ORDER BY wellbeing_index DESC;
```

3. Student working status vs Wellbeing Index and Anxiety Score
 ```SQL
SELECT u.Student_Working_Status,
ROUND(AVG(m.wellbeing_index),2) AS Wellbeing,
ROUND(AVG(m.Anxiety_Score),2) AS Anxiety_Score
FROM users u
JOIN mental_health m ON u.user_id = m.user_id
GROUP BY u.Student_Working_Status
ORDER BY Wellbeing DESC;
```

4. Sleep quality by Student Working Status
```SQL
SELECT u.Student_Working_Status AS Status,
ROUND(AVG(m.sleep_quality_score),2) AS sleep_quality_Score
FROM users u
JOIN mental_health m ON u.user_id = m.user_id
GROUP BY u.Student_Working_Status
ORDER BY sleep_quality_Score DESC;
```

5.Caffeine intake by Gender
```SQL
SELECT u.gender,
ROUND(AVG(Caffeine_Intake_Cups), 2)  AS Avg_Caffeine_Intake_Cups
FROM users u
JOIN engagement_lifestyle e ON u.user_id = e.user_id
GROUP BY u.gender
ORDER BY Avg_Caffeine_Intake_Cups DESC;
```

6. Which country has the highest anxiety score?
```SQL
SELECT u.country,
ROUND(AVG(m.Anxiety_Score),2) AS avg_anxiety
FROM users u
JOIN mental_health m ON u.user_id = m.user_id
GROUP BY u.country
ORDER BY avg_anxiety DESC;
```


### POWER BI DASHBOARD 
KPI Cards
- Average Anxiety Score: Measures overall stress level
- Average Wellbeing Index: Indicates general mental wellness
- Average Screen Time: Tracks digital exposure
- Average Caffeine Intake: Lifestyle stimulant behavior
- Highest Burnout Risk %: Identifies at-risk population
  > 👉 These KPIs provide a quick snapshot of mental health status and lifestyle patterns
   

DASHBOARD CHARTS

- Key Insights

- 😩 Anxiety Score by Gender (Non-Binary gender has the highest Anxiety Score
- 📈 Wellness Level by Sleep Quality Level (Upward Trend between Wellness Level and Sleep Quality Level)
- 👨‍🎓👩‍🎓 Anxiety Level and Wellness Level by Student Working Status (Students has the highest Anxiety Level and the Lowest Wellbeing Level)
- 🛌 Sleep Quality by Student Working Status (Both Status is recorded as the highest with avearge point of 6.59, while working status is 6.50 and student status is 6.47)
- ☕ Caffeine Intake by Gender (Non-Binary Gender has the highest caffeine intake by 34%)
- 🗺 Anxiety Level by Country (Pakistan recorded the highest by 99.8%)


### POWER BI DASHBOARD

<img width="960" height="496" alt="gen z dashboard power bi" src="https://github.com/user-attachments/assets/ceb5a008-6e5d-4120-8664-cef6e502bae5"/>





### KEY QUESTIONS AND INSIGHTS 
1. ❓ Which gender experiences the highest anxiety?

   ✅ Insight:
   - Non-binary individuals show the highest anxiety levels (35%)
     > They also record the highest caffeine intake

   💡 Interpretation:
   - This group may be experiencing higher stress exposure or coping behaviors
 
2. ❓ How does sleep quality affect wellbeing?

   ✅ Insight:
   - A strong upward trend exists between sleep quality and wellbeing
   > Better sleep → higher wellbeing scores
  
   💡 Interpretation:
   - Sleep is a major driver of mental health improvement

3. ❓ Who is more stressed: Students or Workers?

   ✅ Insight:
   - Students have: Highest anxiety levels and the Lowest wellbeing scores

   💡 Interpretation:
   - Academic pressure and uncertainty may significantly impact students

4. ❓ Does sleep differ across student-working groups?

   ✅ Insight:
   - Sleep quality shows only slight differences across groups

   💡 Interpretation:
   - Sleep alone does not fully explain anxiety differences, Other factors (stress, workload) play a role

5. ❓ How does caffeine consumption vary by gender?

   ✅ Insight:
   - Non-binary individuals consume the most caffeine

   💡 Interpretation:
   - Possible link between stress and stimulant use

6. ❓ Which country has the highest anxiety levels?

    ✅ Insight:
    - Pakistan shows the highest average anxiety score (4.8)

    💡 Interpretation:
	 - Cultural, social, or economic factors may influence mental health trends


### KEY TAKEAWAY
	•	📱 Lifestyle factors significantly impact mental health
	•	😴 Sleep quality is strongly linked to better wellbeing
	•	🎓 Students are the most vulnerable group
	•	⚧️ Non-binary individuals show higher stress indicators
	•	🌍 Non-binary individuals show higher stress indicators
	
### INTERACTIVE FEATURES 
To enhance analysis and user experience, I integrated slicers in the dashboard:
 * Age Slicer (Explore how mental varies across age group)
 * Country Slicer (Compare trends across different regions)
> These allows users to dynamically filter insights and uncover deeper patterns


### RECOMMENDATION   
1. 🧠  Target High-Risk Groups
	 Focus mental health support on:
	 * Students
	 * Non-binary individuals


2. 😴 Promote Sleep Awareness
    - Encourage better sleep habits
	- Introduce “digital detox” initiatives


3.  📉  Reduce Stress Triggers
	- Provide stress management tools
	- Encourage healthier coping mechanisms beyond caffeine

4. 📊 Localized Mental Health Strategies
	- Tailor interventions based on country-specific trends



### DATA SOURCE
This data was gotten from Kaggle
[Download here](https://www.kaggle.com/datasets/hammadansari7/gen-z-mental-wellness-and-digital-lifestyle-patterns)

### CONCLUSION
* This analysis highlights that mental health in Gen Z is strongly influenced by lifestyle and demographic factors.
* While sleep quality improves wellbeing, high anxiety levels among students and non-binary individuals suggest a need for targeted mental health interventions and inclusive mental health strategies by leveraging data-driven insights, organizations can design more effective wellness programs that address both behavioral and demographic risk factors.






