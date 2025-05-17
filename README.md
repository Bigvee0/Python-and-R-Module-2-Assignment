San Francisco Salary Analysis
This repository contains a Jupyter Notebook (sf_salary_analysis.ipynb) and an R script (unzip_display.R) to analyze San Francisco salary data from 2011-2018, fulfilling the requirements of the assignment.
Requirements

Python: Python 3.7+ with the following packages:
pandas
numpy
seaborn
matplotlib
zipfile (standard library)


R: R with the readr package
Data File: Total.csv (place it in the same directory as the notebook)

Files

sf_salary_analysis.ipynb: Jupyter Notebook containing Python code for data import, processing, employee details function, error handling, and exporting to CSV/zip.
unzip_display.R: R script to unzip the employee profile and display the data.
Total.csv: The input dataset (not included in the repository; user must provide).
Employee_Profile.zip: Generated zip file containing employee details CSV (created by running the notebook).
pay_distribution.png: Plot of TotalPay and BasePay distributions.
average_pay_by_year.png: Bar plot of average TotalPay by year.

Instructions

Setup:

Ensure Total.csv is in the same directory as sf_salary_analysis.ipynb.
Install required Python packages:pip install pandas numpy seaborn matplotlib


Install R and the readr package:install.packages("readr")




Running the Python Notebook:

Open sf_salary_analysis.ipynb in Jupyter Notebook or JupyterLab.
Run all cells sequentially.
The notebook will:
Load the dataset and convert columns to numeric.
Define a function to retrieve employee details by name.
Process data using a dictionary to calculate average pay by year.
Export employee details (e.g., for 'NATHANIEL FORD') to a CSV file and zip it into Employee_Profile.zip.
Generate and save visualizations (pay_distribution.png and average_pay_by_year.png).


Example usage of the employee details function:details = get_employee_details('NATHANIEL FORD', df)




Running the R Script:

Ensure Employee_Profile.zip is in the same directory as unzip_display.R.
Run the R script:Rscript unzip_display.R


The script will:
Unzip Employee_Profile.zip to Employee_Profile_Unzipped.
Read and display the first CSV file found in the unzipped folder.




Output:

Employee_Profile.zip: Contains the CSV file with employee details.
Employee_Profile_Unzipped/: Directory created by the R script containing the unzipped CSV.
Visualization PNG files in the working directory.



Notes

Error handling is implemented for file loading, invalid employee names, and general exceptions.
The notebook assumes the Total.csv file matches the structure provided in the assignment.
Modify the employee_name variable in the notebook to export details for a different employee.
The R script assumes the zip file contains a single CSV; modify it if multiple CSVs are expected.

Submission
The repository contains all necessary files except Total.csv. To submit:

Run the notebook to generate Employee_Profile.zip and visualization PNGs.
Run the R script to verify unzipping and data display.
Zip the repository (including the notebook, R script, generated zip file, and PNGs) and submit.

