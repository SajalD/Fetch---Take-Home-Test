# Fetch---Take-Home-Test

## First: explore the data

### Code and the output can be seen in the Jupyter notebook attached, following is a summary of basic Exploratory Data Analysis:
#### 1. Products Dataset
##### Missing Values:
- **CATEGORY_1:** 111 missing values  
- **CATEGORY_2:** 1,424 missing values  
- **CATEGORY_3:** 60,566 missing values  
- **CATEGORY_4:** 778,093 missing values (most of the data is missing)  
- **MANUFACTURER:** 226,474 missing values  
- **BRAND:** 226,472 missing values  
- **BARCODE:** 4,025 missing values  

##### Duplicates:
- 215 duplicate product records  


#### 2. Transactions Dataset
##### Missing Values:
- **BARCODE:** 5,762 missing values  

##### Invalid Values in Numeric Fields:
- **FINAL_QUANTITY:** Contains non-numeric values like `'zero'` and `' '`  
- **FINAL_SALE:** Contains blank entries `' '` 

##### Duplicates:
- 171 duplicate transaction records


### 3. Users Dataset
##### Missing Values:
- **BIRTH_DATE:** 3,675 missing values (affects age-based analysis)  
- **STATE:** 4,812 missing values  
- **LANGUAGE:** 30,508 missing values (significant)  
- **GENDER:** 5,892 missing values  

##### Duplicates:
- No duplicate user records detected


### 4. Referential Integrity Issues
- **USER_ID:** 49,738 transactions have `USER_ID`s not found in the Users dataset  
- **BARCODE:** 19,408 transactions have `BARCODE`s not found in the Products dataset

### Second:  provide SQL queries
In this analysis, I used **SQLite3 in Python** to execute SQL queries for exploring and analyzing the data. The datasets are loaded into an SQLite in-memory database for querying. **Query and its output is present in Jupyter notebook as well.**

#### **Closed Ended Questions**
1. What are the top 5 brands by receipts scanned among users 21 and over?
2. What are the top 5 brands by sales among users that have had their account for at least six months?

#### **Open Ended Questions**
2. Which is the leading brand in the Dips & Salsa category?




