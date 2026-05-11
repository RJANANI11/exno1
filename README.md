# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```
import pandas as pd
data=pd.read_csv("C:\\Users\\admin\\Downloads\\SAMPLEIDS.csv")
data
```
<img width="1085" height="711" alt="image" src="https://github.com/user-attachments/assets/7c38f274-5485-435c-9105-45b44a4e04a9" />

```
data.describe()

```
<img width="825" height="296" alt="image" src="https://github.com/user-attachments/assets/a6f3f91f-6e95-4ff5-a8fb-4bdf122a8ca2" />

```
data.isnull()

```
<img width="772" height="521" alt="image" src="https://github.com/user-attachments/assets/49afabd6-7c3d-4487-9b2f-bfdeb4cc6828" />

```
data.isnull().sum()

```
<img width="317" height="285" alt="image" src="https://github.com/user-attachments/assets/cd371b05-5824-4959-b10c-54927f6e1675" />

```
data.notnull()

```
<img width="862" height="580" alt="image" src="https://github.com/user-attachments/assets/66d70507-ba5a-4ace-9f9d-a65b14ede662" />

```
data.notnull().sum()
```

<img width="447" height="306" alt="image" src="https://github.com/user-attachments/assets/e8fd2db9-ab10-40c0-a8d6-5e92d689454c" />

```
data.dropna()
```

<img width="940" height="450" alt="image" src="https://github.com/user-attachments/assets/fcd15c76-1563-4a06-ad45-d74ba5d95941" />

```
data.dropna(axis=1)
```

<img width="772" height="728" alt="image" src="https://github.com/user-attachments/assets/3638d4e3-ac8f-47a6-b1b5-42f3098d49ad" />

```
data
```

<img width="1137" height="743" alt="image" src="https://github.com/user-attachments/assets/25ea44d0-bce1-42fc-9f25-36b084ca9a4d" />

```
data.dropna(inplace=True)
data
```

<img width="952" height="468" alt="image" src="https://github.com/user-attachments/assets/23a89f31-da47-4c6e-96ed-04888e2c5064" />

```
import pandas as pd
data1=pd.read_csv("C:\\Users\\admin\\Downloads\\Loan_data.csv")
data1
```

<img width="1250" height="467" alt="image" src="https://github.com/user-attachments/assets/e2242298-38a8-419d-96d0-ac261847ca25" />

```
data.isnull()
```

<img width="810" height="461" alt="image" src="https://github.com/user-attachments/assets/6ea014b7-bee6-4bf8-8538-1ec05677d84e" />

```
data.isnull().sum()
```

<img width="680" height="302" alt="image" src="https://github.com/user-attachments/assets/d6c5ea6f-679e-4881-903a-195a710d126b" />

```
data.fillna("Datascience")
```

<img width="938" height="481" alt="image" src="https://github.com/user-attachments/assets/3bb8ae32-1468-4aea-a1d8-3d1609b3af45" />

```
data
```

<img width="965" height="477" alt="image" src="https://github.com/user-attachments/assets/241759bf-d0fe-488d-b294-4ca171a54d3d" />

```
data.ffill()
```

<img width="957" height="477" alt="image" src="https://github.com/user-attachments/assets/790993a3-408b-4c7e-9631-fa36cd910288" />


# Result
The given dataset was successfully read and cleaned using Python. Missing values and duplicate records were handled properly, and the cleaned data was saved into a new file named cleaned_data.csv
