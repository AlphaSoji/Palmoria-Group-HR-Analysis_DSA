# Palmoria-Group-HR-Analysis_DSA
## Project Overview:
Paimoria Group has concerns about public perception of its gender diversity posture. The perception is negative. 
Palmoria has therefore commissioned an exploratory analysis of its HR records in order to identify key problem areas, 
and develop mitigants to correct the negative public perception.

**Ancilliary Project:** As an ancilliary, Palmoria has also requested an impact assessment of the recently 
approved bonus package.

## Project Process: 
### 1.	PLAN:
i)	**Tools**

    a) Microsoft Power BI Desktop**: 
      -For Data Extraction, Transformation and Loading (ETL).
      -For DashBoard
      
ii)	**Data Source**:

      -Company HR Data in .csv format. Provided by Palmoria.
      -Company Bonus Rules & Mapping in Excel. Provided by Palmoria.

iii) The Executive Summary/Recommendations to be presented in GitHub.

### 2.	ANALYSE:
i)	**Data Cleaning & Preparation**

    a) Generally, there are two genders in the organization. Some employees refused to disclose their gender. 
       Assign <Nonbinary> gender status to these employees.
    b) Delete some employees that are without salary because they are no longer with the company. 
    c) Delete some employees that are without department because they are no longer with the company. 
    d) Promote Headers.
    e) Check Datatypes and make corrections.
    f) Format Data accordingly. Insert Currency signs and Percentage signs where necessary.

ii) **Exploratory Data Analysis(EDA)**

    a) Transform the Data in the light of the Project Plan to craete new colums or rows necessary for 
       the analysis.
    b) Concatenate Department column and Ratings column in Palmoria Group emp-data.csv file to create 
       Department_Rating column.
    c) Unpivot the Bonus Rules.xlxs file "on other columns".
    d) Concatenate Department column and Ratings column in Bonus Rules.xlxs file to create Department_
       Rating column in Bonus Rules file.
    e) Join Bonus Rules table to Palmoria Group emp-data table on the Department_Rating column which is 
       now common to both tables. 
       This is to ensure that the correct Bonus_rate is assigned to each rating in corresponding departments.
    f) Split the Department_Rating column back to their separate original columns.
    g) With the created Bonus_Rate column, calculate a new column, "Bonus", which is Salary x Bonus_Rate. 
    h) Calculate another column for "Total_pay", which is Salary + Bonus.
    i) Make another colums for the "salary_Band", using the "Conditional Column" menu in the "Add Column" tab.
    
### 3.	CONSTRUCT:

i)	Case Scenario: 
•	Analyse the company data and generate insights that the Palmoria management team would need to address.
•	Your analysis should be visualized using appropriate charts.
•	Your focus should be on gender-related issues within the organization and its regions.
•	The insights required are based on your discretion. However, Mr Gamma, as an insider, has offered to give you pointers on areas you need to pay attention to.
iii)	Pointers From Mr Gamma:

   **1.	What is the gender distribution in the organization? Distil to regions and departments**

        
   **2.	Show insights on ratings based on gender**


   **3.	Analyze the company’s salary structure. Identify if there is a gender pay gap. 
        If there is, identify the department and regions that should be the focus of management.**
        
   **4.	A recent regulation was adopted which requires manufacturing companies to pay employees a minimum of $90,000.**

   **Does Palmoria meet this requirement?**
    
   **Show the pay distribution of employees grouped by a band of $10,000. For example: How many employees fall into a band of $10,000 – $20,000, $20,000 – $30,000, etc.? 
     Also visualize this by regions.**

***iv)	Bonus Case Question:***
    **5.	   Allocating the annual bonus pay to employees based on the performance rating.** 
•	Calculate the amount to be paid as a bonus to individual employees.
•	Calculate the total amount to be paid to individual employees (salary inclusive of bonus).
•	Total amount to be paid out per region and company-wide.

### 5.	EXECUTE:
i.  DashBoard Creation.
Use the cleaned dataset and pivot outputs to build an Excel dashboard. 
ii. Also use the Dashboard to develop a write up or presentation to explain and present your insights and finish with recommendations.
