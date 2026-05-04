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

### TOOLS
- SQL
- Power BI
  
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
- 😊 Wellness Level by Sleep Quality Level (Upward Trend between Wellness Level and Sleep Quality Level)
- 😩 Anxiety Level and Wellness Level by Student Working Status (Students has the highest Anxiety Level and the Lowest Wellbeing Level)
- 🛌 Sleep Quality by Student Working Status (Working Status shows slight differnce amongst all Status as the highest)
- ☕ Caffeine Intake by Gender (Non-Binary Gender has the highest caffeine intake by 34%)
- 😩 Anxiety Level by Country (Pakistan recorded the highest by 99.8%)


### POWER BI DASHBOARD

<img width="960" height="496" alt="gen z dashboard power bi" src="https://github.com/user-attachments/assets/ceb5a008-6e5d-4120-8664-cef6e502bae5" />



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
	
### INTERACTIVE ANALYSIS 
To enhance usability, I integrated Year and Region Slicer, allowing dynamic filtering of the performance metrics across different years and regions. 
This helps uncover;
- Year-over-year performance change
- Shifts in product demand
- Trend Analysis
- Performance tracking by period
- Market growth patterns

### RECOMMENDATION   
1️⃣ 🧠  Target High-Risk Groups
	> Focus mental health support on:
	* Students
	* Non-binary individuals


2️⃣ 😴 Promote Sleep Awareness
	•	Encourage better sleep habits
	•	Introduce “digital detox” initiatives


3️⃣ 📉  Reduce Stress Triggers
	•	Provide stress management tools
	•	Encourage healthier coping mechanisms beyond caffeine

4️⃣ 📊 Localized Mental Health Strategies
	•	Tailor interventions based on country-specific trends



### DATA SOURCE
This data was gotten from Kaggle
[Download here](https://www.kaggle.com/datasets/mohamedamiralkrdawy/bmw-global-sales-analysis-20182025)

### CONCLUSION
* This analysis reinforced an important lesson, Sales performance doesn't exist in isolation, it's influenced by product strategy, economic conditions, and market positioning. The analysis of BMW’s global sales data from 2018 to 2025 shows a steady growth in overall performance, supported by consistent revenue trends and strong market contributions across key regions.
* A major highlight is the significant increase in Battery Electric Vehicle (BEV) share, indicating a clear shift toward electrification. Meanwhile, premium vehicle share remains relatively stable with slight fluctuations, suggesting a gradual evolution in product mix. Additionally, external factors such as rising fuel prices and fluctuating GDP growth provide important context for changing consumer behavior and demand patterns.




