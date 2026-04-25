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
|Age|	Gender| Country | Student_Working_Status|Daily_Social_Media_Hours| Screen_Time_Hours| Night_Scrolling_Frequency| Online_Gaming_Hours| Content_Type_Preference| Exercise_Frequency_per_Week| Daily_Sleep_Hours| Caffeine_Intake_Cups|Study_Work_Hours_per_Day|Overthinking_Score| Anxiety_Score|Mood_Stability_Score|Motivation_Level|Emotional_Fatigue_Score| Wellbeing_Index|Burnout_Risk|
|----|--------|-----|-------|------|-----------|--------------|------------|----------|--------------|-----------|-----------------|
|2019|	1/4/1900|	Wed|	Europe|	MINI|	$2.6K|	$40K|	$105M|	0.06|	17.63|	3.98|	1.04|
|2020|	1/4/1900|	Wed|	USA|	MINI|	$2.5K|	$43K|	$110M|	0.061|	19.81|	3.52|	1.16|
|2018|	1/1/1900|	Sun|	Europe|	MINI|	$2.6K|	$43K|	$110M|	0.013|	19.12|	3.5|	1|
|2021|	1/2/1900|	Mon|	Europe|	MINI|	$2.8K|	$40K|	$113M|	0.084|	15.12|	4.2|	1.14|
|2018|	1/10/1900|	Tue|	China|	MINI|	$2.7K|	$42K|	$114M|	0.025|	19.19|	5.28|	0.92|


[Dataset file showing the pivot tables][bmw_global_sales_2018_2025.xlsx](https://github.com/user-attachments/files/26570700/bmw_global_sales_2018_2025.xlsx)


### DATA CLEANING
- Changed date and amount datatype to date and currency format 
- Removed, duplicate, missing or invalid values

### TOOLS
Excel |Power Query Editor
  
### DASHBOARD 
KPI Cards
1.  Average Anxiety Score: Measures overall stress level
2. Average Wellbeing Index: Indicates general mental wellness
3. Average Screen Time: Tracks digital exposure
4. Average Caffeine Intake: Lifestyle stimulant behavior
5.   Highest Burnout Risk %: Identifies at-risk population
   > These KPIs provide a quick snapshot of mental health status and lifestyle patterns
   

DASHBOARD CHARTS

- 💹 Top model that generated the highest revenue is X7 (Revenue by Model)
- 🚗 Top model that generated the highest unit sold is IX (Unit sold by Model)
- 🗺️ Top selling region is China (Revenue by Region)
- 📊 Regional sales breakdown - Total Revenue by Model and by Region (This shows all models sold in each region and X7 model top in all the regions
- BEV_Share vs Premium Share: This revealed an interesting strategic shift while premium share declined slightly by 2% (-2%YoY), overall revenue increased, supported by a strong 14% YoY growth in BEV_Share
- GDP Growth vs Fuel Price Index: The chart compares the trend of fuel price index and GDP growth from 2018 to 2025

### DASHBOARD

<img width="811" height="459" alt="BMW sales Dashboard" src="https://github.com/user-attachments/assets/59a21d37-aa23-4089-baf2-ba121821fdd6" />


### KEY QUESTIONS AND INSIGHTS 
1. Which gender experiences the highest anxiety?

✅ Insight:
	•	Non-binary individuals show the highest anxiety levels (35%)
	•	They also record the highest caffeine intake

💡 Interpretation:
	•	This group may be experiencing higher stress exposure or coping behaviors


2.  How does sleep quality affect wellbeing?

✅ Insight:
	•	A strong upward trend exists between sleep quality and wellbeing
	•	Better sleep → higher wellbeing scores

💡 Interpretation:
	•	Sleep is a major driver of mental health improvement
	

3.  Who is more stressed: Students or Workers?

✅ Insight:
	•	Students have:
	•	Highest anxiety levels
	•	Lowest wellbeing scores

💡 Interpretation:
	•	Academic pressure and uncertainty may significantly impact students
	
	
4. Does sleep differ across student-working groups?

✅ Insight:
	•	Sleep quality shows only slight differences across groups

💡 Interpretation:
	•	Sleep alone does not fully explain anxiety differences
	•	Other factors (stress, workload) play a role
	

5. How does caffeine consumption vary by gender?

✅ Insight:
	•	Non-binary individuals consume the most caffeine

💡 Interpretation:
	•	Possible link between stress and stimulant use
	
	
6. Which country has the highest anxiety levels?

✅ Insight:
	•	Pakistan shows the highest average anxiety score (4.8)

💡 Interpretation:
	•	Cultural, social, or economic factors may influence mental health trends
	

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
	> Students
	> •Non-binary individuals


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




