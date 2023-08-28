# Data_cleaning
# AIM
    To read the given data and perform data cleaning and save the cleaned data to a file.
# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect,
incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data, but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
STEP 1: Read the given Data STEP 2: Get the information about the data STEP 3: Remove the null values from the data STEP 4: Save the Clean data to the file

# CODE and OUTPUT
# DATA SET:
~~~
import pandas as pd
df=pd.read_csv("Data_set.csv")
print(df)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
df['aired_on']=df['aired_on'].fillna (df['aired_on'].mode()[0])
df['original_network']=df[ 'original_network'].fillna (df['aired_on'].mode()[0])
df.head()
df['rating']=df['rating'].fillna (df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()
df['watchers']=df['watchers'].fillna (df['watchers'].median())
df.head()
df.info()
df.isnull().sum()
~~~
# LOAN DATA:
~~~
import pandas as pd
df=pd.read_csv("Loan_data.csv")
print(df)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['Loan_ID']=df['Loan_ID'].fillna(df['LoanAmount'].mode()[0])
df.head()
df['Dependents']=df['Dependents'].fillna (df['Dependents'].mode()[0])
df.head()
df['Gender']=df['Gender'].fillna (df['Gender'].mode()[0])
df.head()
df['Education']=df['Education'].fillna (df['Dependents'].mode()[0])
df.head()
df['Self_Employed']=df['Self_Employed'].fillna (df['Self_Employed'].mode()[0])
df.head()
df['LoanAmount']=df['LoanAmount'].fillna (df['LoanAmount'].mean())
df.head()
df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean())
df.head()
df['Credit_History']=df['Credit_History'].fillna (df['Credit_History'].median())
df.head()
df.info()
df.isnull().sum()
~~~
# OUTPUT:
# DATA SET:
# DATA:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/b0fe5acd-c841-45fe-a127-470c37d538ce)


# NON NULL BEFORE:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/630aeee1-52d6-4d1e-ac3d-f56789fd799e)


# NON NULL AFTER:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/bff1717b-db04-4ca4-91c3-a27e475d2bff)


# LOAN DATA:
# DATA:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/00491224-140c-472f-bf75-78e8abee7694)


# NON NULL BEFORE:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/c51323cf-27e7-4aba-a422-476d29c3b59f)


# MODE:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/e0e6ecd9-7aad-4eb4-a766-751e78a02e94)


# MEAN:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/8aa205b3-79e9-4b03-a5e9-5a5899b8e034)

![image](https://github.com/212221040181/Data_cleaning/assets/133640291/40a2080d-3a66-4a1c-a49b-1455f371ca43)

![image](https://github.com/212221040181/Data_cleaning/assets/133640291/3436ab73-8441-4405-8589-4e3c52558159)

![image](https://github.com/212221040181/Data_cleaning/assets/133640291/9b02560d-7dd8-457c-b888-2a8213eff0a4)


# MEDIAN:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/0e1453e6-6ed5-401c-95e8-4fcf6dd888a9)

![image](https://github.com/212221040181/Data_cleaning/assets/133640291/74424867-7d2f-4803-899e-cae724b6969e)

![image](https://github.com/212221040181/Data_cleaning/assets/133640291/46f3879a-ac6d-4179-8613-b7ad94c59114)


# NON NULL AFTER:
![image](https://github.com/212221040181/Data_cleaning/assets/133640291/b09b3de9-d282-40e7-a4d2-4b0ad89199a6)
