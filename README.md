# Advanced Statistics (DS3001) 
## Project Proposal 

### Research Question: How do various organizational, personal, and environmental factors contribute to different patterns of employee absenteeism?

### Project Overview
##### This repository contains code and analysis for exploring patterns in workplace absenteeism using advanced statistical techniques. The project analyzes a real-world dataset from a courier service firm (2007-2010) to understand behavioral factors behind employee absences and identify predictive patterns.

### Introduction
##### Employee absenteeism—defined as frequent, often unplanned absences from work without valid cause—has become a growing concern for organizations globally. This project explores the multidimensional drivers of absenteeism, including health issues, family obligations, and workplace factors.
##### The economic impact is significant:
##### 1. U.S. employers lose an estimated $225 billion annually
##### 2. European economies face costs of up to 2.5% of GDP
##### Despite these costs, organizations often struggle to identify root causes and build effective, data-driven attendance strategies. Our analysis aims to provide actionable insights through statistical modeling and exploratory techniques.

### Dataset Description
##### The dataset contains 740 instances of employee absences with 21 attributes collected over three years (July 2007 – July 2010) from a courier company. Variables include:
##### 1. Employee Information: ID, age, tenure at the company (service time), education level, and disciplinary records
##### 2. Absence Details: Month and day of absence, reason for absence (classified under the International Classification of Diseases - ICD), and total absenteeism time (in hours)
##### 3. Workplace Factors: Daily workload, achievement of performance targets, transportation expenses, and distance from residence to work
##### 4. Health & Lifestyle Factors: BMI, weight, height, smoking and drinking habits, number of children, and number of pets
##### 5. Environmental Factors: Season and weekday of absence

### Research Questions
##### - What individual, health-related, and organizational factors are most strongly associated with chronic absenteeism?
##### - How do different variables interact to influence absence duration and frequency?
##### - Can absenteeism behavior be reliably predicted and classified using statistical models?

### Methodology
##### Data Preprocessing

##### 1. Conversion of categorical variables (Reason for absence, Seasons, Social drinker)
##### 2 Handling of missing values and placeholder entries
##### 3. Feature engineering for analysis

##### Statistical Analysis 

##### - Distribution Analysis: Shapiro-Wilk test for normality assessment
##### - Regression Modeling: Negative Binomial regression for count data with overdispersion
##### - Hypothesis Testing: Mann-Whitney U test and Kruskal-Wallis test for non-parametric comparisons
##### - Classification: Multiclass logistic regression to categorize absence patterns

##### Visualization Techniques

##### - Histograms and Q-Q plots for distribution analysis
##### - Correlation heatmaps for relationship exploration
##### - Box plots and grouped mean plots for categorical comparisons
##### - Bar plots for frequency analysis

### Key Findings
##### Health-Related Absences:
##### - ICD-related absences, while less frequent (262 vs 478 non-ICD instances), result in significantly longer durations (p < 0.001)
##### - Significant variation in absence duration across different illness categories, with cardiovascular (Reason 9) showing substantially longer absences

##### Commute Distance and Transportation:
##### -Contrary to expectations, commute distance did not significantly impact absenteeism
##### -Similar transportation expenses between employees commuting <40km (Rs. 217) and ≥40km (Rs. 229) suggest possible company subsidies

##### Family Responsibilities:
##### -Each additional child associated with approximately 20.57% increase in absenteeism time (p < 0.001)
##### -Parents show significant absence spikes during March, May, and July, likely coinciding with school holidays

##### Absenteeism Patterns
##### Identified three distinct absenteeism profiles:
##### -Chronic: High frequency or total hours
##### -Occasional: Moderate frequency and total hours
##### - Minimal: Low frequency and total hours
#####   *Chronic absentees use varied reasons (reason consistency = 0.32), while minimal absentees consistently cite the same reason (reason consistency = 0.64)

##### Limitations
##### - Dataset from a single courier company in Brazil (2007-2010), limiting generalizability
##### - Lack of direct measures for job satisfaction, mental health, and precise organizational policies
##### - Weak linear correlations between predictors and absenteeism hours
##### - Strong right-skewness and overdispersion in the data


### Contributors

##### Lakshay Aggarwal (U20230111)
##### Niyati Singh (U20230080)
##### Sara Goyal (U20230019)
##### Preesha Katial (U20030057)
##### Rohan Sharma (U20230012)
