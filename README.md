# Prime or Not

A simple program to determine whether a given number is a prime number or not.

## What is a Prime Number?
A prime number is a whole number greater than 1 that is divisible only by 1 and itself.

Examples:
- 2, 3, 5, 7, 11, 13 are prime numbers
- 1, 4, 6, 8, 9, 12 are not prime numbers

## Project Goal
This project checks whether the user-entered number is:
- Prime
- Not Prime

## How It Works
1. If the number is less than or equal to 1, it is not prime.
2. Check divisibility from 2 up to the square root of the number.
3. If it is divisible by any value in that range, it is not prime.
4. Otherwise, it is prime.

## Example
Input: 17

Output: Prime

Input: 18

Output: Not Prime

## Usage
Run the program and enter a number.

Example in Python:
```python
num = int(input("Enter a number: "))

if num <= 1:
    print("Not Prime")
else:
    is_prime = True
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            is_prime = False
            break
    if is_prime:
        print("Prime")
    else:
        print("Not Prime")
```

## License
This project is open for learning and modification.
