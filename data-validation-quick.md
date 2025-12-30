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
