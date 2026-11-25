# Excel Pro – Spreadsheet Practice Workbook

## Overview
This workbook is an Excel practice project containing student grades, logical tests, sales calculations, and employee data. It demonstrates common Excel formulas for calculations, conditional logic, dates, and text manipulation.

## Workbook Sheets

### 1. Students Grade
Contains student records with:
- Student ID and student name
- Marks in Math, Science, and English
- Enrollment date
- Average score
- Grade

**Formulas used**
- `AVERAGE` and `ROUND` – calculate the average of the three subject marks and round it to one decimal place.
- Nested `IF` – assign a letter grade based on the average:
  - A: 90 and above
  - B: 75–89.9
  - C: 60–74.9
  - D: 50–59.9
  - F: below 50

### 2. Sheet2
Contains logical checks linked to the **Students Grade** sheet:
- `Math & Science>80` – returns Yes when both Math and Science marks are greater than 80.
- `Subject<50` – returns Yes when at least one of Math, Science, or English is below 50.

**Formulas used:** `AND`, `OR`, and `IF`.

### 3. Sales Data
Contains sales records with:
- Sales ID, product, region, and salesperson
- Sales amount and date
- Discount percentage and discount amount
- Net amount
- Eligibility status

**Formulas used**
- Nested `IF` – calculates the discount rate:
  - 15% for sales of 40,000 or more
  - 10% for sales of 25,000 or more
  - 5% for sales of 10,000 or more
  - 0% for lower sales
- Multiplication – calculates the discount amount.
- `ROUND` – calculates the rounded net amount after discount.
- `OR` and `IF` – marks a sale eligible when the amount is at least 25,000 or the product is Laptop.

### 4. Employee Data
Contains employee records with:
- Employee ID, name, department, salary, and joining date
- Joining year and month
- Tenure and days employed
- First name and uppercase/lowercase name
- Rounded, ceiling, and floor salary values

**Formulas used**
- `YEAR` – extracts the joining year.
- `TEXT` – displays the joining month as an abbreviated month name.
- `TODAY` and `DATEDIF` – calculate completed years of tenure, with a check for future joining dates.
- Date subtraction – calculates days employed, with a check for future joining dates.
- `LEFT` and `FIND` – extracts the first name.
- `UPPER` and `LOWER` – changes name capitalization.
- `ROUND`, `CEILING`, and `FLOOR` – rounds salary values using the specified increments.

## How to Use
1. Open `Excel pro.1.xlsx` in Microsoft Excel or a compatible spreadsheet application.
2. Select the required worksheet using the sheet tabs.
3. Review the sample records and formulas.
4. To test the formulas, change an input value such as a mark, sales amount, joining date, or salary.
5. If formulas do not update automatically, set calculation mode to **Automatic** or recalculate the workbook.

## Notes
- Formula results may recalculate when the workbook is opened in Excel.
- The employee tenure and days-employed calculations use `TODAY()`, so their results change with the current date.
- This README describes the workbook structure and formulas present in the supplied spreadsheet.
