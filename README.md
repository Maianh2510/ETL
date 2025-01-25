### HR Analytics: Job Change of Data Scientists ##
**Intorduction**

A company which is active in Big Data and Data Science wants to hire data scientists among people who successfully pass some courses which conduct by the company.

Many people signup for their training. Company wants to know which of these candidates are really wants to work for the company after training or looking for a new employment because it helps to reduce the cost and time as well as the quality of training or planning the courses and categorization of candidates.

Information related to demographics, education, experience are in hands from candidates signup and enrollment.

**Data details**

Source: Swiss coding academy

The main goal: Our primary objective is to perform ETL (Extraction, Transformation, Loading) on six data tables in five formats: Google Sheets, Excel, CSV, a database, and a website table.

**We need to answers below to find main goal:**

1. What does raw data look like?
   
2. How do I know if I need to etl data? and why?
   
3. What if the data is misformatted and missing data?
    
4. How to combine data from files?
    
5. How to load files?

**We need to do:**

First, We need to import library

*1. What does raw data look like?*

Step 1 : Load data

Step 2 : View 5 first row of data

Via these two steps revealed the raw data.

*2. How do we know if we need to ETL data? and why?*

Step 3 : I checked the data information. As a result, we need to clean the data in the tables. 

Because, this will ensure consistency and uniformity, enhancing data accuracy. Subsequently, we can create visualizations, model the data, and support sound business decisions.

*3. What if the data is misformatted and missing data?*

Step 4 : After step 3, I have handled the following for values ​​that are not in the correct format or are missing:
In Table 1 : Enrollies' data
# Fill null value in column gender by  other

df['gender'] = df['gender'].fillna('other').str.lower()

df['full_name'] = df['full_name'].fillna('unknown').str.lower()

df['city'] = df['city'].fillna(df['city'].mode()[0]).str.lower()

# convert column gender to category

df['gender'] = df['gender'].astype('category')

df['full_name'] = df['full_name'].astype('string')

df['city']=df['city'].str.lower().astype('category')

**Please see the attached file for my work.**







