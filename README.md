# Attendance Anomaly Detector (Operational Risk)

## Problem Statement

In organizations, irregular attendance and frequent late arrivals can impact productivity and operations.
Manually identifying attendance issues from raw data is time-consuming and error-prone.

## Solution

This project analyzes employee attendance data from an Excel file and classifies each employee into **Low**, **Medium**, or **High operational risk** based on simple, explainable rules.

## Input

* **attendance.xlsx**

  * Contains employee attendance details:

    * Name
    * Total working days
    * Days present
    * Late marks

## Output

* **attendance_report.txt**

  * A text report showing the attendance risk level for each employee.

## Business Rules Used

* Attendance below 75% → High Risk
* Late marks greater than 5 → Medium Risk
* Otherwise → Low Risk

## Technologies Used

* Python
* Excel (openpyxl)

## How to Run

1. Install required library:

   ```
   pip install openpyxl
   ```
2. Place `attendance.xlsx` in the project folder.
3. Run the script:

   ```
   python attendance_analyzer.py
   ```
4. Check the generated `attendance_report.txt` file for results.

## Use Case

This analysis helps operations and support teams proactively identify attendance-related risks and take corrective actions.
