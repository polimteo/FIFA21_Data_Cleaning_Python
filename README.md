Introduction
-
This dataset contains 18,979 records with information about football players, their abilities, and performance, updated up until 2021.

Objective
-
The goal is to clean and enhance the dataset using Python, ensuring accuracy and consistency before proceeding to the data analysis phase.

Data Cleaning Summary
-

Several issues were resolved in this dataset:


**Missing values**
  
- The 'Loan Date End' and 'Hits' columns contained missing values.
- In the 'Loan Date End', the dates represent when the contracts for players on loan would end, while blank entries indicate players who are either free agents or under a regular contract. Therefore, these missing values are valid.
- In the 'Hits' column, missing values indicate that players haven't been searched in the database. These blanks were replaced with 0, and the data type was changed to integer.
  
**Inconsistent formatting of data.**
  
- The 'Heights' and 'Weights' columns had values in different units, which required standardization.
- In the 'Value', 'Wage', and 'Release Clause' columns, there were mixed data formats, with prefixes ('€') representing euros and suffixes ('M' and 'K') representing millions and thousands, respectively.
- I standardized these values using transformations, lambda functions, and data normalization techniques, ensuring they are in the correct data type.

  
**Symbols or characters.**

- In the 'IR', 'SM', and 'W/F' columns, star symbols (★) represented ratings. These symbols were removed, and the values were converted to numeric data types.
- For the 'Club' column, newline characters were removed to maintain a clean format.





