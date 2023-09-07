# KPMG-Virtual-Internship
The dataset referred to here is the dataset furnished for an internship project in collaboration with KPMG. This dataset encompasses information derived from Sprocket Central Pty Ltd, an imaginary enterprise engaged in the global sale of bicycles and cycling-related accessories to its customer base.

# Code Overview
Code Overview: This script operates on data retrieved from a file named "KPMG.xlsx," creating three distinct variables corresponding to three different sheets: "transaction," "CustomerDemographic," and "CustomerAddress."

For the "transaction" data frame, the code addresses missing values, eliminates rows with null brand entries, and fills null values in the "online_order" column with its mode.

Within the "CustomerDemographic" data frame, the code standardizes gender labels (F to Female, M to Male, and U to Unspecified), removes the "default" column, eliminates rows with "deceased_indicator" marked as "Y," rectifies a spelling error in the "job_industry_category," and handles null values in the "job_industry_category" column. It determines the percentage of missing values in this column and fills them using a specified approach: Manufacturing and Financial Services are filled with the most frequent values, while Health and Retail receive half of the remaining null values. Additionally, the code addresses missing values in the "tenure" column by replacing them with the median.

Notably, the "CustomerAddress" data frame is read without any modifications.
