g# Data Validation – Quick Revision

## Purpose
Restrict wrong data entry.

## Steps
1. Select cells
2. Data tab → Data Validation
3. Choose rule:
   - Whole number
   - Decimal
   - List
4. Set condition
5. OK

## Example (Dropdown) 
Allow → List
Source → Yes,No

## Use Case
Avoid typing mistakes.

## IF THERE ARE BLANKS IN DATA AND YOU WANT TO REPLACE WITH 0 
NOW SELECT THE COLUMN ABOVE THEN CHECK ALL THE ENTORE COLUMN FROM TOP TO DOWN ARE SELECTED AND 
PRESS -- CTRL + G 
CLICK SPECIAL
SELECT BLANKS THEN OK 
THEN IT WILL SELECT WHICH ARE HAVING BLANKS THEN IN FORMULA BARS WROTE 0 AND PRESS CTRL+ENTER

Ctrl + F == WHEN YOU ENTER CTRL + F THEN IT ASKS WHAT TO FINF BEFORE DOING THAT CHECK ALL IN A COLUMN EVERY THING IS SELECTED OR NOT THEN TYPE WHAT TO FIND NEXT TYPE WHAT TO REPLACE IN COLUMNS EVERY THING IS 
REPLACED 

##🔹 REAL EXAMPLE (ACCIDENT DATA)
🚗 Accident Data in Excel
Accident_ID	  State	          Year	     Deaths
101	      Andhra Pradesh	   2022	       15
102	       Telangana	      2022	       20
101	      Andhra Pradesh	   2022	       15
103	       Tamil Nadu	      2022	       25

🔴 Problem:
Accident_ID 101 is repeated → Deaths counted twice 
HOW TO DO == Ctrl + A + DATA + REMOVE DUPLICATES + YOU WILL SEE LIKE   ☑ Accident_ID ☑ State ☑ Year ☑ Deaths THEN CLICK OK  DUPLICATES REMOVED OK 
BY THE ABOVE ONE I HAVE A DOUBT THAT IN THE TABLE THERE IS 2022 ALSO REPEATED THEN Y IT IS NOT REMOVING EXCEL CHECK ROW BY ROW 
Row 1:
101 | Andhra Pradesh | 2022 | 15
Row 3:
101 | Andhra Pradesh | 2022 | 15 -- AFTER CHECKING ROW1 AND ROW3 EXCEL FINDS AND REMOVE ONE THIS IS THE CHECKING PROCESS 

## TRIM
Formula:

=TRIM(A1)

Example:
" Andhra " → "Andhra"

When to use:
✔ Grouping errors
✔ Filter not working properly

## CLEAN (Remove Hidden Characters)

Purpose: Remove non-printable characters

Formula:

=CLEAN(A1)
❌ Before CLEAN (Problem)

Cell A1 contains:

Andhra↵
↵ = hidden line break (not visible in Excel)

✅ After CLEAN (Result)
Output:
Andhra

## We can also use clean+trim 
Use TRIM + CLEAN together:
=TRIM(CLEAN(A1))

## Text to Columns
📌 Purpose

Splits one column into multiple columns based on a delimiter
(like -, ,, space, tab, etc.)

❌ Before (Problem)

Single column A contains:

Andhra Pradesh - NH16V

All information is in one cell ❌
Hard to analyze, filter, or group.

🔹 How to Use (Step-by-Step)

Select the column (A)

Go to Data → Text to Columns
Choose Delimited
Click Next
Select delimiter → -
Click Finish

✅ After (Result)
State	            Road
Andhra Pradesh	   NH16

## Delete Irrelevant Columns
📌 Purpose
Remove columns that are not needed for analysis or dashboard.

Home → Delete → Delete Sheet Columns
🔎 Example (Clear)
❌ Before
State	   Accidents	Deaths	Remarks
AP	         120	    45	   Verified
✅ After
State	 Accidents	Deaths
AP	      120	      45
Here which column you want to delte that mention properly

## Data Validation
These can be used in so many ways like making the numbers as list and to make a security like deaths >=0 when we enter -5 it is not valid 

Data → Data Validation

✅ Example 1: Deaths ≥ 0 (No negative values)
❌ Problem

Someone may enter:
-5
Which is invalid ❌

✅ Steps to Apply Validation

1️⃣ Select the Deaths column
2️⃣ Go to Data → Data Validation
3️⃣ Under Allow, choose:
Whole numbers
4️⃣ Under Data, choose:
greater than or equal to

5️⃣ Enter:
0
6️⃣ Click OK
