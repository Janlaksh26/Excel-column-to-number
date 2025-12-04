# Excel-column-to-number
Python code  to print Excel-style column number  (A-1,AA-27,BNM-1729)

This repository contains a python program to print the column name in excel style 
#How it works

Excel columns follow a base 26 letter system:
A-1
B-2
AA-27
BNM-1729

The python script calculates the numeric value for any given column name.

#How to run
python excel.py

#example
Input:TYU
Output:14191

#How This Code Works
Function defined: excel_col_num(col_name) accepts a column name as input.
Convert to uppercase: Ensures input is case-insensitive.
Initialize result: result = 0 will accumulate the final number.
Loop through each character in the string.
For each character:
Convert letter to a number using ASCII:
value = ord(i) - ord('A') + 1
Update result using base-26 math:
result = result * 26 + value<


#Why Base-26?

Excel columns work like a number system with 26 symbols (A–Z).
Example:
A = 1
Z = 26
AA = 1×26 + 1 = 27
AB = 1×26 + 2 = 28
Return the result once all characters are processed.

