                                                                                                                                                                                                                                                           HR Analytics Report
Overview
The HR Analytics report analyzes employee behavior, attrition trends, performance metrics, and engagement factors using data-driven insights. Key findings reveal that low job satisfaction, lower income, and poor work-life balance contribute significantly to attrition, while higher performance ratings and career progression opportunities enhance retention. Salary disparities and workload management also impact employee satisfaction. The report provides actionable recommendations, including targeted retention programs, competitive compensation structures, enhanced training, and engagement strategies to improve overall workforce stability and productivity.

Objectives
1.	Clean and preprocess the dataset for reliable analysis.
2.	Perform Exploratory Data Analysis (EDA) to understand dataset structure and key patterns.
3.	Identify trends, correlations, and key drivers influencing employee attrition and satisfaction.
4.	Visualize findings effectively using Matplotlib and Seaborn.
5.	Provide actionable insights to help HR management improve employee retention and engagement.

Dataset
The dataset includes the following key attributes:
1.	Employee Information:
•	EmployeeID – Unique identifier for each employee.
•	Age – Age of the employee.
•	Gender – Male/Female/Other.
•	Department – Department where the employee works.
•	Job Role – Specific role/title of the employee.
•	Tenure – Number of years the employee has worked in the company.
2.	Job Satisfaction & Work Conditions:
•	Job Satisfaction – Satisfaction level (scale 1-4).
•	Work-Life Balance – Rating of work-life balance (scale 1-4).
•	Job Involvement – Level of job involvement.
•	Overtime – Whether the employee works overtime (Yes/No).
3.	Compensation & Benefits:
•	Monthly Income – Salary received per month.
•	Hourly Rate – Pay per hour.
•	Stock Option Level – Level of stock options granted.
•	Percent Salary Hike – Salary increment percentage.
4.	Performance & Career Growth:
•	Performance Rating – Employee's performance score.
•	Training Hours – Number of training hours attended.
•	Years Since Last Promotion – Time since the last promotion.
•	Job Level – Employee’s job position level.
5.	Attrition & Retention Indicators:
•	Attrition – Whether the employee left the company (Yes/No).
•	Num Companies Worked – Number of companies the employee has worked for.
•	Years at Company – Total years with the current employer.
•	Years in Current Role – Time spent in the current job role.

Project Workflow
•	Data Collection & Preprocessing
1.	Load dataset using Pandas.
2.	Handle missing values and duplicates.
3.	Convert categorical data using encoding techniques.
•	Exploratory Data Analysis (EDA)
1.	Summarize numerical & categorical attributes.
2.	Identify trends in employee attrition, satisfaction, and performance.
3.	Perform correlation analysis to find key relationships.
•	Data Visualization
1.	Use Matplotlib & Seaborn for histograms, boxplots, heatmaps, and bar charts.
2.	Visualize attrition patterns, salary distributions, and performance trends.
•	Key Insights & Findings
1.	Identify high-risk attrition factors (e.g., low salary, poor work-life balance).
2.	Determine the impact of satisfaction, compensation, and training on retention.
•	Recommendations & Actionable Insights
1.	Suggest strategies to reduce attrition and improve engagement.
2.	Provide HR policy improvements based on data-driven findings.
•	Final Deliverables
1.	Jupyter Notebook with analysis & visualizations.
2.	Comprehensive report with insights & recommendations.

Handling Missing Data:
.	Implement strategies like mean/median imputation for numerical values.
.	Use mode imputation for categorical values.
.	Remove records with excessive missing values.

Exploratory Data Analysis (EDA) – HR Analytics

EDA helps in understanding the dataset’s structure, distributions, and key patterns related to employee behavior, attrition, and performance.
1. Data Overview:
•	Loaded dataset using Pandas and checked its structure (df.info(), df.describe()).
•	Identified missing valuess and handled them appropriately.
•	Renamed columns for consistency.


2. Employee Distribution Analysis:
•	Department & Job Role: 
o	Visualized employee count across departments using bar charts.
o	Identified departments with higher attrition rates.
•	Age & Salary Distributions: 
o	Used histograms and box plots to analyze age and salary spread.
o	Detected salary discrepancies across job roles.


3. Attrition Analysis:
•	Attrition vs. Job Satisfaction & Work-Life Balance: 
o	Employees with low job satisfaction and poor work-life balance showed higher attrition rates.
o	Used box plots & count plots for visualization.
•	Attrition vs. Salary & Tenure: 
o	Employees with lower salaries and fewer years in the company had higher turnover.


4. Correlation Analysis:
•	Heatmap Visualization using Seaborn to find relationships between: 
o	Job satisfaction, income, performance ratings, and attrition.
o	Workload & tenure impact on employee retention.
6. Performance & Engagement Analysis:
•	Training & Performance Trends: 
o	Employees with more training hours generally had higher performance ratings.
•	Promotion & Career Growth: 
o	Employees with fewer promotions over time were more likely to leave.



Analysis         
Descriptive Analysis 
	Descriptive Analysis Using Pandas and NumPy: 
Computed summary statistics for numerical and categorical variables to understand data distribution. Converted numeric columns to appropriate types using pd.to_numeric() and categorized categorical columns using .astype('category'). Generated descriptive statistics for both data types. (Applied: df.describe() for numerical & categorical summaries, df.dtypes to check data types).


	Categorical Variable Summary: 
Analyzed unique value counts for all categorical columns to understand data diversity and distribution. (Applied: df[col].nunique() for counting unique values in categorical columns).


Visualization of Employee Distribution
	Visualization of Employee Distribution: Created bar charts to analyze the distribution of employees across departments. Used sb.countplot() to visualize employee counts, customized labels, and applied plt.xticks(rotation=45) for better readability. (Applied: sb.countplot() for bar chart, plt.grid(axis='y') for clarity).


	Salary Distribution Analysis: Used a histogram to visualize the distribution of monthly income and detect skewness or outliers. Applied sb.histplot() with bins=30 and kde=True for smooth density estimation. (Applied: sb.histplot() for histogram visualization).


Correlation Analysis
	Correlation Analysis: 
Computed the correlation matrix for numerical variables to identify relationships between key attributes. Used sb.heatmap() to visualize correlations with annotations and a color gradient for better interpretation. (Applied: df.corr() for correlation matrix, sb.heatmap() for visualization). 


Atrition Analysis
	Attrition Segmentation: 
Analyzed job satisfaction, monthly income, and performance rating differences between employees who left and those who stayed. Used sb.boxplot() to compare distributions across attrition status. (Applied: sb.boxplot() for job satisfaction, income, and performance rating segmentation).


	Attrition Trends Across Demographics:
 Calculated attrition rates for different demographic groups (age, gender, department, education, and job role) to identify high-risk categories. Used df.groupby() with a lambda function to compute attrition percentages and visualized trends using sb.barplot(). (Applied: calculate_attrition_rate() for computation, sb.barplot() for visualization).


Conclusion - HR_Data Analysis Report
•	Low job satisfaction, lower income, and poor work-life balance are key factors driving employee attrition.
•	Employees with higher performance ratings and career growth opportunities are more likely to stay.
•	Limited promotions and stagnant salaries increase the likelihood of employee turnover.
•	Training, compensation, and work environment strongly influence retention and engagement.
•	Targeted HR strategies such as improving compensation, offering career development programs, and enhancing work-life balance can reduce attrition and boost productivity.
•	Implementing data-driven HR policies will help create a more stable and motivated workforce.

