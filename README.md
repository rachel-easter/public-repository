# Employee Work Analysis

This Python script analyzes an input file containing employee timecard data and identifies employees who meet specific criteria related to their work hours. The script prints the names and positions of employees who:

1. Have worked for 7 consecutive days.
2. Have less than 10 hours of time between shifts but greater than 1 hour.
3. Have worked for more than 14 hours in a single shift.

## Usage

1. **Install Dependencies:**

   Before running the script, make sure you have the necessary dependencies installed. You can install them using pip:

   ```bash
   pip install pandas openpyxl
Run the Script:

Make sure to provide the correct file path to the input Excel file in the script.

Execute the script:

bash
Copy code
python employee_work_analysis.py
View the Results:

The script will analyze the input file and print the results to the console.

Output:

The script will also generate an output.txt file containing the same results.

Assumptions
The input file is an Excel file with specific column names:

"Employee Name"
"Position ID"
Hours worked columns from index 4 to 10 (inclusive) for 7 days.
The script uses regular expressions to extract time values, assuming they are in the format "HH:MM."

The script assumes that the input file contains relevant data in the specified columns.

Example Input File
The script assumes an input Excel file with the following structure:

Employee Name	Position ID	...	Day 1	Day 2	Day 3	Day 4	Day 5	Day 6	Day 7
John Doe	123	...	08:00	08:15	08:30	08:45	09:00	09:15	09:30
Jane Smith	456	...	07:45	08:00	08:15	08:30	08:45	09:00	09:15
...	...	...	...	...	...	...	...	...	...
License
This project is licensed under the MIT License - see the LICENSE file for details.

