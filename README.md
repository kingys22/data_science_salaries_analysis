# Data Science Salaries Analysis 
## An overview and analysis of the "Data Science Salaries 2023" dataset found on Kaggle

**TABLE OF CONTENTS**
- Overview of The Data
- Cleaning/Modifying The Data
- Analysis
- Conclusion

Check out the dataset [**HERE**](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023?resource=download).

# Overview of The Data
The dataset consists of information about data science professionals and their salaries. There are over 3000 records with 10 fields. 

1. work_year: The year the salary was paid. 
2. experience_level: The experience level in the job during the year. 
3. employment_type: The type of employment for the role.
4. job_title: The role worked in during the year.
5. salary: The total gross salary amount paid.
6. salary_currency: The currency of the salary paid as an ISO 4217 currency code.
7. salaryinusd: The salary in USD.
8. employee_residence: Employee's primary country of residence in during the work year as an ISO 3166 country code.
9. remote_ratio: The overall amount of work done remotely.
10. company_location: The country of the employer's main office or contracting branch.

# Cleaning/Modifying The Data
The final dataset contains these fields after all changes. Everything in **bold is changed or new**.

1. work_year: The year the salary was paid. 
2. **experience_level**: The experience level in the job during the year.
3. **employment_type**: The type of employment for the role.
4. job_title: The role worked in during the year.
5. **job_group**: The function of their role separated into 4 groups. 
6. salary_in_usd: The salary in USD.
7. **mean_income**: The average income in the respective country. 
9. **employee_location**: Employee's primary country of residence in during the work year.
10. **company_location**: The country of the employer's main office or contracting branch.
11. remote_ratio: The overall amount of work done remotely.


**Changelog (in order of fields)**
- experience_level: Converted abbreviations in old dataset to their unabbreviated form. (e.g. SE = Senior Level)
- employment_type: Same change as above. (e.g. FT = Fulltime)
- job_group: New Field. Attached b1-b4 depending on the job function. Function divided into 4 groups - Data Analysis (b1), Data Science (b2), Data Engineering (b3), and Miscellaneous (b4).
-  mean_income: New Field. Referenced the world banks average gni per capita per country as a marker for mean income. World Bank data [here](https://data.worldbank.org/indicator/NY.GNP.PCAP.CD).
-  employee_location & company_location: See below

* For the fields mean_income, employee_location, and company_location all records were converted into their full country name using the ISO country code table found [here](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes). Additionally, for the mean_income field, ensured that all country names from the world bank data and the ISO country code were identical. Manually changed the ones that were not consistent.


# Analysis
Analysis Contents                

1- Where are most data professionals from?


2- Exploring the remote work ratio.

3- Which job function do most data professionals serve as?

4- Is there a difference in salary between job functions?

# Conclusion

