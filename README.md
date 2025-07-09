# prodigy-infotech-task-1
This repository is about a task which i was asked to perform for my virtual internship at prodigy infotech.

Task 1 Create detailed test cases in markdown format for a calculator taht performs add, subtract, multiply, and divide operations.Focus on valid inputs (e.g. positive and negative numbers, decimals, BODMAS)and invalid inputs(e.g. non- numeric characters ,division by zero).Each test case should include the following elements 

Test Case 1: Addition with Positive Numbers

•	Test Case ID: TC_ADD_01
•	Test Description: Verify addition of two positive integers
•	Preconditions: Calculator application is open
•	Test Steps:
1.	Enter 5
2.	Press +
3.	Enter 7
4.	Press =
•	Expected Result:
•	Display shows 12
________________________________________

Test Case 2: Subtraction with Negative Result

•	Test Case ID: TC_SUB_01
•	Test Description: Verify subtraction resulting in a negative number
•	Preconditions: Calculator application is open
•	Test Steps:
1.	Enter 3
2.	Press -
3.	Enter 8
4.	Press =
•	Expected Result:
•	Display shows -5
________________________________________

Test Case 3: Multiplication with Decimals

•	Test Case ID: TC_MUL_01
•	Test Description: Verify multiplication of decimal numbers
•	Preconditions: Calculator application is open
•	Test Steps:
1.	Enter 2.5
2.	Press ×
3.	Enter 4
4.	Press =
•	Expected Result:
•	Display shows 10
________________________________________

Test Case 4: Division by Zero

•	Test Case ID: TC_DIV_01
•	Test Description: Verify division by zero handling
•	Preconditions: Calculator application is open
•	Test Steps:
1.	Enter 9
2.	Press ÷
3.	Enter 0
4.	Press =
•	Expected Result:
•	Display shows error message like "Cannot divide by zero" or "Error"
________________________________________

Test Case 5: Invalid Input (Non-numeric Characters)

•	Test Case ID: TC_INV_01
•	Test Description: Verify error for non-numeric input
•	Preconditions: Calculator application is open
•	Test Steps:
1.	Enter abc
2.	Press +
3.	Enter 5
4.	Press =
•	Expected Result:
•	Display shows error message like "Invalid input" or "Error"
________________________________________

Test Case 6: BODMAS/Order of Operations

•	Test Case ID: TC_BODMAS_01
•	Test Description: Verify evaluation follows BODMAS rule
•	Preconditions: Calculator application is open
•	Test Steps:
1.	Enter 2
2.	Press +
3.	Enter 3
4.	Press ×
5.	Enter 4
6.	Press =
•	Expected Result:
•	Display shows 14 (since multiplication is performed before addition: 2+(3×4)=142+(3×4)=14)
_________________________________________________________________________________________________________
Test Case 7. Division with Decimal Result
•	Test Case ID: TC_DIV_02
•	Description: Verify division resulting in a decimal value.
•	Steps:
1.	Enter 5
2.	Press ÷
3.	Enter 2
4.	Press =
•	Expected Result: Display shows 2.5
_________________________________________________________________________________________________________

Test Case 8. Large Number Calculation
•	Test Case ID: TC_LARGE_01
•	Description: Verify handling of very large numbers.
•	Steps:
1.	Enter 999999999
2.	Press +
3.	Enter 1
4.	Press =
•	Expected Result: Display shows 1000000000 (or handles overflow gracefully if applicable).
________________________________________________________________________________________________________

