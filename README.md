# PROJECT-BANK
**INTRODUCTION**
We're using data from 100 different customers, Our goal is to look at different variables to know who would be a good candidates for loans. We're not just looking at how much money someone has. We're also considering things like where they live, their behavior, and other factors. This way, we can really understand if someone is reliable when it comes to paying back loans. We are focused on  making our decisions more accurate. This helps us use our resources better and lowers the chances of something going wrong. At World Street Bank, we're all about using data to make fair, clear, and efficient decisions about credit.

**TYPE OF DATASET AND SOURCE**
https://www.kaggle.com/code/prashantsparhad/bank-card-prediction/input
The original data set had 10127 rows, but as we wanted to explore in detail the differences of our customer we decided to selected only a sample of 100. This dataset is composed by 21 columns that add information about our customers, for us the mos relevant one are 11:
- ClientNum (integer): An integer that serves as a unique client identification. 
- Attrition_flag (categorical): Denotes if the client is a current client or one who has attrition. This variable is classified. 
- Customer_age (integer): An integer indicating the customer's age.
- Gender (categorical): The customer's gender, indicated as either Male (M) or Female (F).
- Dependent_count (integer): The number of the customer's dependents, from 0 to 5.
- Education_level (categorical): A string indicating the customer's level of education.
- Marital_status (categorical): The customer's marital status, which can be either married, single, unknown, or divorced.
- Income_category ($): The customer's income category, expressed in US dollars. The summary omits any mention of the precise income brackets or
  groups.
- Card_Category (categorical): The customer's credit card type, with the options of Blue, Silver, or Other.
- Months_on_book (integer): This variable indicates how long the consumer has been a client, in months, between 13 and 56.
- Credit_limit ($): The customer's credit limit expressed in US dollars. There is a specified range of $1440 to $34,500.

**BASIC INFORMATION**
- Number of rows and columns = (100, 27)
- Data type: these 6 variables are the only ones with strings: Attrition Flag, Gender, Education_Level, Marital_Status,
  Income Category, Card Category and the rest of the variables are integers.

**DETAILS ON THE INVESTIGATION**

The primary objective of this project is to identify ideal candidates for granting loans and credit within the bank's customer base. We will focus on predicting customer creditworthiness and assessing the risk of loan defaults.

  **Inputs**: The program will require access to confidential customer data from “The World Street Bank”, including historical account data for 100 customers.
  
  **Outputs**: The program will generate a report containing insights, visualisations, and recommendations for granting loans and credit to specific customers.
  
  **Packages We Will Use**: The program is going to be runed in Python and we are going to use the Pandas and Matplotlib.

**DESIGN OF THE DATASET**

First, we will clean and preprocess the dataset, to address missing values and outliers, ensuring data quality. 
We will analyse the data to gain insights into customer characteristics and identify patterns. 

  - First we clean rows and we have just left with 100 clients.
    
  - We change these 6 variables from string to integer category: Attrition Flag, Gender, Education_Level, Marital_Status,
  Income Category, Card Category.

**CODE IN PYTHON TO MAKE THE NUMERICAL VARIABLES:**

  1.1. Download Python and pycharm (link pycharm) (https://www.python.org/downloads/) into your desktop.
  2.  Importing Necessary Library:The script begins by importing the pandas library
     Pip install pandas and import pandas as pd.
  3. Loading the CSV File: The code reads the "projectbank.csv" file into a DataFrame
     using the read_csv function from pandas.
  4. Download the code from the “CODING.py” folder.
  5. Defining Mapping Dictionaries:Several mapping dictionaries are defined to convert categorical values into numerical          representations. Each dictionary corresponds to a specific categorical column in the dataset and the code uses the map       function from pandas to create new numerical columns in the DataFrame based on the mapping dictionaries.
  
  6. Saving the Updated DataFrame to a New CSV File:Finally, the code saves the updated DataFrame to a new CSV file
      named"updated_projectbank.csv" using the to_csv function.


**GRAPHICS FOR EXPLAINIG THE DATASET**

Barchart attrition number x count:

<img width="385" alt="image" src="https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/45c1ab55-d9b3-40ed-87fb-514d139a36ba">

Bar chart income category and customer Age by Gender: 

<img width="287" alt="image" src="https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/5c99f6b8-490a-450e-a1d3-e848f35573c7">

Barchart Income Category Number x Count

![image](https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/69843844-a93f-4c64-9921-c1d5e1262c35)


Barchart Education level:

![image](https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/f40f1fcf-f73a-43bf-86b6-0752856f132b)

**EXPLAINING THE CODE OF THE GRAPHS**
1. Once you have clean the dataset and add the new variables.
2. Install 2 libraries: pip install matplotlib, pip install pandas in the terminal
3. import pandas as pd import matplotlib.pyplot as plt
4. Download the code from the “CODINGRAPHS” folder
5. upload the updatedfolder: https://docs.google.com/spreadsheets/d/18y78HwFkJX4VpXCnKNzlubgCz9f3Hal5WUf4RVspoco/edit#gid=0
   
<img width="227" alt="image" src="https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/868f9ef1-83d6-444e-b4d6-4610e1d3a55b">

6. Save “CODINGRAPH” in a folder that you choose to be the directory of your project in Pycharm.
   Once you have saved it, open this file in Pycharm by clicking on the directory, then clicking “New” and finally clicking
   “File” and type in the name of the file, in this case: “CODINGRAPHS.py”.

**MOCKUPS**
![image](https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/597850fd-28f3-4f5b-8ebd-244561e651b5)

**RESULT**

This bank wants to make sure that the loans that are going to be give away are also going to be given back, therefore 
first we are going to leave just the 10 most loyal clients, for that we are first going to see in a graph the relationship between months_on_book (time in months) and total_relationship_count (relationship with the bank) and take out the 10most loyal. Secondly with the most 10 loyal clients we are going to just focus on the clients that have an income of more than 60k.

**GRAPH OF THE RESULT**

barchart of loyalty: months_on_book and total_relationship_count:

<img width="452" alt="image" src="https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/dd35b27a-4600-4424-a2ee-6f0a5d75ab0f">

chart with the most 10 loyal customers and their income:

<img width="169" alt="image" src="https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/464754e5-070b-4908-a569-8936eeeeb31a">

**EXPLAINING THE CODE OF THE RESULT**
1. Once you have clean the dataset and add the new variables.
2. Install 2 libraries: pip install matplotlib, pip install pandas in the terminal
3. import pandas as pd import matplotlib.pyplot as plt
4. Download the code from the “CODINGRESULT” folder
5. upload the updatedfolder: https://docs.google.com/spreadsheets/d/18y78HwFkJX4VpXCnKNzlubgCz9f3Hal5WUf4RVspoco/edit#gid=0
   
<img width="227" alt="image" src="https://github.com/mariamartinezgonzalez/PROJECT-BANK/assets/151723296/868f9ef1-83d6-444e-b4d6-4610e1d3a55b">

6. Save “CODINGRESULT” in a folder that you choose to be the directory of your project in Pycharm.
   Once you have saved it, open this file in Pycharm by clicking on the directory, then clicking “New” and finally clicking
   “File” and type in the name of the file, in this case: “CODINGRESULT.py”.





