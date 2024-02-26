# Exploratory Data Analysis(EDA)

## Common Data Abbreviation
## Column
Column(structured data in the form of a table) is known by 3 most common names **Feature/Attribute/Variable**. A column can be age, gender, etc.

## Rows
In structured data rows are also called observations, instance, and data point.

## What is EDA
The process of exploring and summerizing the main characteristics of the data to uncover **patterns, relationships** and **trends**.
It helps in formulating questions and making data-driven decisions.
According to my research, companies that are not data-driven, meaning companies that don't make decisions on logic and reasoning with respect to data, are doomed to fail sooner or later.

## Importance of EDA
- provides **initial understanding** of dataset.
- Helps in identifying data **quality issues**, such as **missing values, outliers** and **inconsistencies**.
- Guides the selection of appropriate statistical techniques and **models**.
- Helps in feature engineering and **variable selection**.
- Enables the discovery of **meaningful insights** and actionable conclusions.
**Example**, Nadra data represents garbage data or data that is not understandable through EDA most of Nadra dataset is improved and plenty or almost all garbage data is removed.

## Steps in EDA
- Data Cleaning
- Descriptive Statistics
- Data Visualization
- Data Distribution
- Correlation Analysis
- Outlier Detection
- Data Transformation
 
### Descriptive Statistics
Descriptive Statistics also known as **Summary Statistics**. Summary Statistics is done through **Measure of Central Tendency**(on average value e.g Voters age average), **Measure of Dispersion**(e.g using age attribute, how to check how many people will give me vote, we cannot say age 16 voter will vote for me because obviously his not eligible currently. Using Standerd Deviation we can find this that 18 years old could vote for me but let's say something complex 18 years old, 30 years old 50 years old(when data is dispersed alot) which will vote for me. This is done by using Stats).

**In Simple Words** Descriptive Statistics is the branch of statistics that focuses on summarizing and describing the main features/attributes/variables of a dataset.

### Data Distribution
Normally Distribution is something when something is in a range for example there can be some students with A+ and some with F while there will be a line of B+. Some times there is **Bias** in Data Distribution for example one student is passed while other all students are failed, so Biasing is something that doesnot tell the whole story for example if a student failed that does'nt mean that he is unintelligent.

#### How to do Data Distribution
It is done through Plotting and checking through it the quality of data through Data **Visualization**. We can use **Pandas** to achieve this task.

### Correlation Analysis
Studying the relationship of 2 columns(**Feature, Attribute, Variable**) is known as Correlation Analysis. If values of both columns are increaing than we have positive Correlation Analysis. While if one Feature values are increasing while other feature values are decreasing than we have negative Correlation Analysis. If there is no relation found than we can say the relationship is **Undeterred** or **not found**.

### Data Transformation
Data Transformation is important as most models love numbers.

### Data standardization
Data Standardization is a type of data preprocessing that makes different features have a **same scale**.


<img width="320" alt="image" src="https://github.com/AbdulHadi806/Machine-learning-Basic-notes/assets/113926529/f17cfcfe-e678-4f15-8e38-7426300a6293">


### Why we care about Dispersion?
- Increased difficulty in **capturing patterns**.
- Increased risk of **overfitting**.
- Reduced predictive **accuracy**.
- Impact on **outlier handling**.  
