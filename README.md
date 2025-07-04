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
    Here is the Transformed Dataset
        https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Transformed%20DATASET.xlsx
    
### 3.	CONSTRUCT:

   **1.	What is the gender distribution in the organization? Distil to regions and departments**

       a) Company Total: 946. Male 465(49%). Female 441(47%). Nonbinary 40(4%).
        https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/1.%20Gender%20Distribution%20in%20the%20organisation.png
       
       b) By Region: Kaduna 361. Abuja 335. Lagos 250.
       Kaduna: Male 182(50%). Female 165(46%). Nonbinary 14(4%).
       https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Kaduna%20Distribution.png
       Abuja: Male 159(48%). Female 158(47%). Nonbinary 18(5%).
       https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Abuja%20Distribution.png
       Lagos: Male 124(50%). Female 118(47%). Nonbinary 8(3%).
        https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Lagos%20Distribution.png

     c) By Department:
         Accross all the deparment, the same proportional deistribution of gender was maintained. Departmental majority was 
         alternated between Male and Female gender from department to department e.g. While Male had majority in Production and Legal departments; Female had majority in             Human Resources, Services and Research departments.
         https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Department%20Distribution.png
    
   **2.	Show insights on ratings based on gender**

        44% - 420 people were rated Average. 19% - 180 rated Good. 14% - 131 rated Poor. 10% - 90 rated Very Good. 6% - 54 People rated Very Poor. 8% - 71 were Unrated.
        This same partern of ratings holds true accross the board for all the genders. 

   **3.	Analyze the company’s salary structure. Identify if there is a gender pay gap. 
        If there is, identify the department and regions that should be the focus of management.**

        There is no Gender pay gap in the company. The aggregated salary for Male was $34.8million and Female $31.8million. This could easily be explained by head count            difference between the 2 genders( Male: 465. Female: 441). The same applies to the Nonbinary staff: Just 4% of total. Nonbinary salary is also about 4% of total.
        
   **4.	A recent regulation was adopted which requires manufacturing companies to pay employees a minimum of $90,000.**

   **Does Palmoria meet this requirement?**

   No. Palmoria does not meet the $90,000 minimum wage requirement. The average salary accross board is $73,700. Which less than $90,000. Only the Accounts department in      Lagos have an average salary of $93,500 (Slightly above the minimum wage).
       
       - Overall.
       https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Overall%20compared%20to%20minimum%20wage..png
       - Lagos.
       https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Lagos%20compared%20to%20minimum%20wage..png
        
   **Pay distribution of employees grouped by a band of $10,000. For example: How many employees fall into a band of $10,000 – $20,000, 
       $20,000 – $30,000, etc.?**

***iv)	Bonus Assignments:***
    **5.Allocating the annual bonus pay to employees based on the performance rating.** 
   
    a) Amount to be paid as a bonus to individual employees.
    b) Total amount to be paid to individual employees (salary inclusive of bonus).
    c) Total amount to be paid out per region and company-wide.

   **There are SLICERS and CARDS in the DASHBOARD that clearly show all the above**

### 5.	EXECUTE:
**i.  DashBoard** 
https://github.com/AlphaSoji/Palmoria-Group-HR-Analysis_DSA/blob/main/Palmoria%20HR%20DashBoard.png

**Transformed Dataset**

**Summary and recommendations**

ii. Also use the Dashboard to develop a write up or presentation to explain and present your insights and finish with recommendations.
