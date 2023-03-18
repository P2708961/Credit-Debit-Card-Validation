# 1 Overview

## 1.1 Why Credit Card Validation is Useful
Credit-card validation is crucial in e-commerce as it helps prevent fraud and ensures that transactions are processed accurately. By validating credit card numbers, e-commerce websites can verify the authenticity of the card and prevent unauthorised purchases. This not only protects the merchants from chargebacks but also enhances the trust of customers in the website. Hence, having a robust credit-card validation system is essential for the success of any e-commerce business.

## 1.2 Potential Stakeholders
Some potential stakeholders for a program like this are as follows:

- E-commerce websites that process payments
- Credit card companies that issue credit cards
- Customers who use credit cards for online transactions
- Regulatory bodies that oversee e-commerce transactions and financial institutions.

## 1.3 Projected Outcomes
Some basic goals that a credit card validation program may need to have are:

- To ensure that the credit card number is in the correct format
- To check the validity of the credit card number by verifying its checksum
- To determine the type of credit card (e.g., Visa, Mastercard, American Express, etc.)
- - -
# 2 Functionality
## 2.1 Validity of Credit Cards
One way to check the validity of a credit card number is by using Luhn's algorithm. The algorithm is named after its creator, Hans Peter Luhn, who developed it in the 1950s.

The algorithm works by taking the credit card number and performing a series of mathematical operations on it. The result is a single digit number that is used to validate the credit card number.

To apply Luhn's algorithm, the following steps can be followed:

1. Starting with the second to last digit and moving backwards, double every other digit.
2. If the result of doubling a digit is greater than 9, then add the digits of the result together (e.g. 7 x 2 = 14, 1 + 4 = 5).
3. Add up all the digits in the credit card number.
4. If the sum of the digits is divisible by 10, then the credit card number is valid.

For example, let's say we want to check the validity of the credit card number 4111 1111 1111 1111. Applying Luhn's algorithm, we get:

  4   1   1   1   1   1   1   1   1   1   1   1   1   1   1   1
  8   1   2   1   2   1   2   1   2   1   2   1   2   1   2   1
  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --
  32  1   2   1   2   1   2   1   2   1   2   1   2   1   2   1
