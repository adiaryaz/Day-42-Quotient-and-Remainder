# Day-42-Quotient-and-Remainder

Day 42/100 - Python Program To Find Quotient And Remainder Of Two Number

# Find Quotient and Remainder

A program to divide two numbers and calculate both the integer quotient and the remainder, while safely handling undefined mathematical operations.

## 📝 Description

This program prompts the user to input two integers: a numerator (the number being divided) and a denominator (the number dividing by). It then performs division to determine the quotient and the remainder.

Instead of using standard division (`/`) which results in a floating-point decimal, this script relies on two specific Python operators:

1. **Integer Floor Division (`//`):** Calculates the quotient by dividing the numbers and discarding any fractional remainder.
2. **Modulo (`%`):** Calculates only the remainder of the division.

Crucially, the program implements defensive programming by checking if the denominator is `0` before performing any calculations. This prevents the system from crashing due to a mathematical `ZeroDivisionError`.

---

## 🎯 Problem Statement

### Input:

* **Input 1:** An integer representing the `numerator` (dividend).
* **Input 2:** An integer representing the `denominator` (divisor).

### Output:

* If the denominator is valid (non-zero): Two formatted strings stating "The quotient is: [quotient]" and "The remainder is: [remainder]".
* If the denominator is zero: An error message stating "Division by zero is not allowed."

### Rules:

1. The program must accept two integer inputs from the user.
2. The program must evaluate if `denominator == 0`. If true, print the error message and bypass the calculations.
3. If the denominator is valid, calculate the quotient using the `//` operator.
4. Calculate the remainder using the `%` operator.
5. Print both the quotient and the remainder on separate lines using f-string formatting.

---

## 💡 Examples

### Example 1 (Standard Division with Remainder)

**Input:**

```
10
3

```

**Output:**

```
The quotient is: 3
The remainder is: 1

```

**Explanation:** 10 divided by 3 goes in exactly 3 times ($3 \times 3 = 9$). The leftover remainder to reach 10 is 1.

### Example 2 (Perfect Division)

**Input:**

```
20
5

```

**Output:**

```
The quotient is: 4
The remainder is: 0

```

**Explanation:** 20 is a multiple of 5. It divides perfectly 4 times with a remainder of 0.

### Example 3 (Zero Division Error handling)

**Input:**

```
15
0

```

**Output:**

```
Division by zero is not allowed.

```

**Explanation:** The program intercepts the 0 denominator at the `if` statement, printing the safe error message instead of crashing the Python interpreter.

### Example 4 (Numerator smaller than Denominator)

**Input:**

```
4
7

```

**Output:**

```
The quotient is: 0
The remainder is: 4

```

**Explanation:** 7 goes into 4 zero times. The entire numerator (4) is passed back as the remainder.

---

## 🚀 How to Use

1. **Clone this repository** (or save the script)

```bash
git clone https://github.com/adiaryaz/Day-42-Quotient-and-Remainder.git
cd quotient-and-remainder

```

2. **Run the program**:

```bash
python main.py

```

Enter the numerator and denominator when prompted to safely calculate the division results.

