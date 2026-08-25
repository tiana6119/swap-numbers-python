# swap-numbers-python
📌 Problem Statement
Swap the values of two numbers using two methods:
1. With a 3rd (temporary) variable.
2. Without a 3rd variable.



❓ Questions & Answers

 1. How do you swap using a 3rd variable?
You create a temporary variable (like `temp`) to hold the first number so it doesn't get lost when you overwrite it:
* `temp = num1`
* `num1 = num2`
* `num2 = temp`

 2. How do you swap without a 3rd variable?
* **Method A (Pythonic way):** Use tuple unpacking: `num1, num2 = num2, num1`
* **Method B (Math way):** Use addition and subtraction:
  * `num1 = num1 + num2`
  * `num2 = num1 - num2`
  * `num1 = num1 - num2`


 💻 Python Code

```python
num1 = 10
num2 = 20

 1. With a 3rd variable
temp = num1
num1 = num2
num2 = temp
print("Swapped with temp:", num1, num2)

 Reset numbers
num1, num2 = 10, 20

2. Without a 3rd variable
num1, num2 = num2, num1
print("Swapped without temp:", num1, num2)
