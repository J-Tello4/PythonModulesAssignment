# Mastering Python Loops Assignment

## Exercise 1: Basic Loop Structures

Understanding the basics of loops is essential for iteration in Python.

- **Task 1.1:** Write a `while` loop that prints the numbers 1 through 10.
- **Task 1.2:** Write a `for` loop that prints each character in the string `"Python"`.
- **Task 1.3:** Create a `for` loop that iterates over a list of numbers and prints the square of each number.

# Task 1.1
digit = 1
while digit <= 10:
    print(digit)
    digit +=1
# Task 1.2

str_ = "python"

for char in str_:
    print(char)

# Task 1.3

list_number = [2, 4, 6, 8, 10]
for number in list_number:
    print(number ** 2)





## Exercise 2: Controlling Loop Flow

`break` and `continue` statements can modify the flow of loops.

- **Task 2.1:** Write a `while` loop that stops printing numbers from 1 to 10 when the number reaches 7 using the `break` statement.
- **Task 2.2:** Write a `for` loop that skips printing the number 5 when iterating over numbers 1 through 10 using the `continue` statement.


# excercise 2.1 code:

digit = 1
while digit <= 10:
    print(digit)
    if digit == 7:
        break
    digit += 1

# excercise 2.2 Code: 
for number in range(1, 11):
    if number == 5:
        continue
    print(number)



## Exercise 3: Nested Loops

Nested loops allow for more complex iterations and data processing.

grid_list = [
[[0,0],[0,1],[0,2]],
[[1,0],[1,1],[1,2]],
[[2,0],[2,1],[2,2]]
]
_CHALLENGE_

- **Task 3.1:** Write a nested `for` loop that prints a 3x3 grid of numbers (i.e., rows and columns of numbers from 0 to 2).
  ^^ skip task 3.1
- **Task 3.2:** Using nested loops, write a program to print the multiplication table for numbers 1 through 5.








## Exercise 4: Looping with Ranges

The `range()` function is a useful tool for generating sequences of numbers in loops.

- **Task 4.1:** Write a `for` loop that prints only the even numbers from 1 to 20 using the `range()` function.
- **Task 4.2:** Write a `for` loop that counts down from 10 to 1 using the `range()` function.

# Excercise 4.1 code:
for numbers in range(0, 21, 2):
    print(numbers)

# Excercise 4.2 code: 
for numbers in range(11,0, -1):
    print(numbers)



## Exercise 5: Real-World Applications of Loops

Loops can be applied in real-world scenarios for tasks like data processing or automation.

- **Task 5.1:** Write a `for` loop that asks the user to input 5 different names and stores them in a list. Then, print each name.
- **Task 5.2:** Write a `while` loop that keeps asking the user to guess a secret number until they get it right. Use `break` when they guess correctly.


# 5.1 code task: 

names_listed = []
for _ in range(5):
    name = input("Please enter a name: ")
    names_listed.append(name)

for name in names_listed:
    print(name)


# 5.2 code task:

number = 77

while True:
    guessing_number = int(input("Type any number: "))
    if guessing_number == number:
        print("You guessed right!!")
        break
    else:
        print("Sorry, keep guessing.")