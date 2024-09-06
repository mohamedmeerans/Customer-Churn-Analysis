

**Dashboard** - https://app.powerbi.com/groups/me/reports/b54d8046-fed4-4e78-a29b-afaf23db66b0/716455551d5482d5eeba?experience=power-bi


**BANK CUSTOMER CHURN ANALYSIS - POWERBI**

**PROJECT OBJECTIVE :**

The objective of a Bank Churn Customer Analysis project using Power BI is to identify, understand, and mitigate factors that contribute to customer churn in a banking environment. By leveraging historical customer data and business Intelligence tools are used .

***TOOLS & TECHNOLOGIES USED:**

   MS EXCEL 
   
   POWER BI 
   
   
   --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
****DATASET : ********

   We have Dataset in the format of CSV. which contains Fields like 
   1. Customer Id
   2. Credit Score 
   3. Country
   4. Gender
   5. Age
   6. Tenure 
   7. Account Balance 
   8. Product Number 
   9. Credit Card 
   10. Active Member 
   11. Estimated Salary
   12. Churn

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**STEP : 1**

**DATA CONNECTION :**

Establish a connection between source file to Power Bi Connectors. while using GET DATA - CSV . once we select the source file format power bi Gets data and uploading , start load data to server.

![CSV](https://github.com/user-attachments/assets/1d39df01-97cd-4f7a-a458-7d9d60d8354d)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**STEP : 2**

**DATA PREPARATION :** 

Data Cleaning and Data Modelling Which plays major role in Dashboard Preparation process. Need to Find unwanted Fields to be Removed and Null Values, Empty Values to be cleaned By Using Power Query Editor.

- Removed Estimated Salary Fields which will not give sense to our Analysis.
- Rename Fields which we need to do analysis. 
- Have To Make Age Group. Grouping The people belongs to specific age range. 
- Change the Data Type which helps to make Measure .

![removed estmated salary](https://github.com/user-attachments/assets/fa4a852e-65d5-41fc-a40c-c8e8ec1b2475)

- If bank Customer Had Credit Card means we can set field value as Owned - 0 . else Not Owned - 1 Represent
-  Churned - 0 , 1 Means Not Churned 
- then Based on Credit score we can make that Group Range - Column named as Credit Score Group.

![churn](https://github.com/user-attachments/assets/5b9fbb3c-d78c-4efa-a968-fe4a13d5b7b7)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**3. DATA MODELLING :**

   based on Dataset , for analysis we can make and derive data tables using Joins Function, Conditional Columns, DAX Measures can create more Data Tables .

1.- ******AGE GROUP** - Represents Age From 
            
            Age Group Id 1 - Less Than 20 Years
            Age Group Id 2 Represent 21 - 30 Years 
            Age Group Id 3 Represent 31 - 40 Years 
            Age Group Id 4  Represent 41 - 50 Years 
            Age Group Id 5 Represent  51 - 60 Years 
            Age Group Id 6 Represent 61 - 70 Years 
            Age Group Id 7 Represent 71 & Greater Years 

![AGE GROUP](https://github.com/user-attachments/assets/96269f23-bc8a-43b6-a793-989a1474a21e)

2. **Credit Score Group**  - Represent Range Of Credit Scores 

            Credit Score Id 1 - Less Than 400
            Credit Score Id 2 - 401 - 500
            Credit Score Id 3 - 501 - 600
            Credit Score Id 4 - 601 - 700
            Credit Score Id 5 - 701 - 800
            Credit Score Id 6 - Above 801

![credit score](https://github.com/user-attachments/assets/d2c0b92c-749c-4b94-a500-cb3a2763c69c)

3. ****Account Balance Group** - Represent Range of Account Balance 

            Account Balance Id 1 - 0 Balance 
            Account Balance Id 2 - 1 - 1k Balance 
            Account Balance Id 3 - 1k - 10k Balance 
            Account Balance Id 4 - 10k - 100k Balance
            Account Balance Id 5 - 100k - 200k Balance  
            Account Balance Id 6 - 200k ABove Balance 

![act balance group](https://github.com/user-attachments/assets/a2c484ac-8725-42c1-99bd-00e03e4ac291)
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**4. Creating Measure Using DAX :**

         Measure to Calculate Churn Rate
         Measure to Calculate Number Of Customers in bank
         Measure to Find How Many Customers we Lost 
         Find Target Churn Rate 
         Minimum Churn Rate 
         Maximum Churn Rate 

![NO Cust Have](https://github.com/user-attachments/assets/b964e652-e079-4ddc-84e9-f09ecf0adbc4)


![No Cust Lost](https://github.com/user-attachments/assets/45be96f2-83a3-4708-9f73-49df80265fe9)

![Churn Rate](https://github.com/user-attachments/assets/095aeab6-beef-469a-bd3a-8016324d8e1d)

-----------------------------------------------------------------------------------------------------------------

**5. Data Visualization :** 

**INSIGHGTS :**

****CARDS : ****
       It helps to Display the Numeric values. 

             1. Displaying Number Of Customers Bank Hold.
             2. Displaying Number of Customer We Lost - Churn Rate
             In Percentage Format.
             3. Guage Represents - Target Churn Rate 

![Card](https://github.com/user-attachments/assets/8b117ea4-e38c-4c2b-a446-c2e13802a4b4)


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
             
**Line Chart  :** 

            1. Product Selected by Customers and Their Counts 
            Have 4 Products 
                 Prod  1 - 5100
                 Prod  2 - 4600
                 Prod  3 - 300
               
![Product](https://github.com/user-attachments/assets/e57a8341-02e9-4234-9f26-4e8a6ea30cd8)


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**DONUT CHART :** 
 
           1. Number of Customer By Genders (Male, Female) - 54 % Customers are Male.  

![Donut](https://github.com/user-attachments/assets/9adf51fa-0929-49fe-afe1-02460e38f574)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**PIE CHART :**

          Number Of Customers in Active State - 50 % Are Active and 50% Are INACTIVE 

  ![piechart](https://github.com/user-attachments/assets/9106e8a9-3947-4874-bddf-de5dab86260c)

  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**TABLE CHART :**

          It Displays Account Balance Group , Based on Number of Customers in Bank. 
           Another Table Represent Number of Customers Belonging Different Countries. 

![Table](https://github.com/user-attachments/assets/ee62b63a-fc6a-40d2-a28b-d56d8179b624)

![Country](https://github.com/user-attachments/assets/5b5b5121-832c-438c-be7a-cbbea736ab27)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**STACKED COLUMN CHART :** 

             It Displayed Number of Customers Having Credit card and Number of Customers Not Owned Credit Card.

![image](https://github.com/user-attachments/assets/22113657-23d7-4a3a-af70-90adbbd9803d)


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**LINE AND CLUSTER COLUMN CHART :** 

            Displays Age Group of Customers and Credit Score Group of Customers count.


![image](https://github.com/user-attachments/assets/f575af99-aa21-46c3-a2ba-4bbb087002b6)


![image](https://github.com/user-attachments/assets/9bc37f45-f5c0-4f1b-9bb4-ea6c5ae035d9)
























