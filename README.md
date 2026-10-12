Customer CSV Data Processor

A Python project for processing customer data from CSV files, validating records, filtering customers, sorting purchase amounts, and exporting summary reports to JSON.

Features

- Read customer records from CSV files.
- Validate age and purchase amount values.
- Handle invalid numeric data using exception handling.
- Filter customers by city and minimum age.
- Sort eligible customers by purchase amount in descending order.
- Generate a summary report with customer count, total purchase amount, and highest-purchase customer.
- Export reports to JSON and verify saved data by reading it back.
- Handle missing input files with an error message.

Technologies

- Python
- CSV and JSON
- File handling
- Exception handling
- Data filtering and sorting

Input Format

The CSV file should contain these columns:

"name", "age", "city", "purchase_amount"

Example:

name,age,city,purchase_amount
Priya,25,Hyderabad,120
Rahul,30,Hyderabad,300

Filtering Rules

The current example selects customers from Hyderabad aged 25 or above, with purchase amounts of zero or greater. Records with invalid numeric values are skipped.

These rules can be changed to match client requirements.

Output

The summary report includes:

- Total eligible customers
- Total purchase amount
- Highest-purchase customer
- Sorted customer records

The report is exported to JSON.

How to Run

1. Open the project notebook in Google Colab or Jupyter Notebook.
2. Make sure the required CSV file is available in the working directory.
3. Run the notebook cells in the correct order.
4. Review the filtered records and generated JSON report.

Error Handling

The project demonstrates handling missing CSV files and invalid numeric values.

Limitations

This is a learning project demonstrating practical Python data processing. Additional automated tests and configurable file paths may be useful before production use.
