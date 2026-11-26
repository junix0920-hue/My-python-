
print("=====================================================") 
print("==========PYTHON PROGRAMMING LEARNING SYSTEM=========")
print("==========FUNDAMENTALS OF PROGRAMMING================")
print("=====================================================")

def show_header():
    print("\n" + "=" * 55)
    print("          PYTHON PROGRAMMING LEARNING SYSTEM")
    print("             FUNDAMENTALS OF PROGRAMMING")
    print("=" * 55)
    print("              CHOOSE WHAT YOU WANT TO LEARN")
    print("=" * 55)


def show_menu():
    print("""
 [1]  Introduction to Programming
 [2]  What is Python Programming?
 [3]  Python Syntax
 [4]  Print Statement
 [5]  Python Comments
 [6]  Variables and Constants
 [7]  Variable Naming Rules
 [8]  Assigned Values and Output Variables
 [9]  Basic Data Types
 [10] Arithmetic Operators
 [11] Expressions and PEMDAS
 [12] Accepting User Input
 [13] Converting Data Types
 [14] Conditional Statements
 [15] Relational Operators
 [16] Logical Operators
 [17] Introduction to Iteration
 [18] For Loop
 [19] While Loop
 [20] While True

 [21] PYTHON QUIZZES AND ACTIVITIES

 [0] EXIT PROGRAM
 """)


print("===================================================")
print("=======================LESSONS=====================")
print("===================================================")
def lesson(choice):

    lessons = {

1: """
LESSON 1: INTRODUCTION TO PROGRAMMING

Programming is the process of giving instructions
to a computer to perform a specific task.

Examples:
- Websites
- Mobile applications
- Computer games
- Management systems

Example:
print("Hello, World!")
""",

2: """
LESSON 2: WHAT IS PYTHON PROGRAMMING?

Python is a high-level programming language.

WHY LEARN PYTHON?

1. Simple and easy to learn.
2. Readable syntax.
3. Beginner-friendly.
4. Used in different fields.
5. Large programming community.

Example:
print("Welcome to Python!")
""",

3: """
LESSON 3: PYTHON SYNTAX

Syntax refers to the rules used to write
a correct Python program.

IMPORTANT RULES:

1. Python is case-sensitive.
2. Use proper indentation.
3. Follow correct spelling.
4. Use correct punctuation.

Example:
name = "Juan"
print(name)

Remember:
name and Name are different.
""",

4: """
LESSON 4: PRINT STATEMENT

The print() function displays information
on the computer screen.

Example:
print("Hello!")
print("Python Programming")
print(100)
print(10 + 5)

OUTPUT:
Hello!
Python Programming
100
15
""",

5: """
LESSON 5: PYTHON COMMENTS

Comments are notes written inside a program.

Python ignores comments when executing code.

SINGLE-LINE COMMENT:

# This is a comment
print("Hello!")

MULTI-LINE COMMENT:

'''
This is a multi-line comment.
'''

Comments help programmers understand their code.
""",

6: """
LESSON 6: VARIABLES AND CONSTANTS

A variable stores information in a program.

Example:
name = "Juan"
age = 18

print(name)
print(age)

CONSTANT:

A constant is a value intended not to change.

Example:
PI = 3.1416
""",

7: """
LESSON 7: VARIABLE NAMING RULES

RULES:

1. Start with a letter or underscore.
2. Do not start with a number.
3. Do not use spaces.
4. Variable names are case-sensitive.
5. Use descriptive names.

CORRECT:
student_name = "Maria"
age = 18
total_score = 95

INCORRECT:
1name = "Juan"
student name = "Maria"
""",

8: """
LESSON 8: ASSIGNED VALUES AND OUTPUT VARIABLES

The assignment operator (=) gives a value
to a variable.

Example:
name = "Maria"
age = 18

print(name)
print(age)

MULTIPLE VARIABLES:

a = "I"
b = "LOVE"
c = "PYTHON"

print(a, b, c)

OUTPUT:
I LOVE PYTHON
""",

9: """
LESSON 9: BASIC DATA TYPES

Python has different data types.

1. STRING (str)
   name = "Juan"

2. INTEGER (int)
   age = 18

3. FLOAT (float)
   grade = 89.5

4. BOOLEAN (bool)
   is_student = True

Example:
print(type("Juan"))
print(type(18))
print(type(89.5))
print(type(True))
""",

10: """
LESSON 10: ARITHMETIC OPERATORS

Arithmetic operators perform calculations.

+   Addition
-   Subtraction
*   Multiplication
/   Division
//  Floor Division
%   Modulus
**  Exponentiation

Example:
a = 10
b = 5

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
""",

11: """
LESSON 11: EXPRESSIONS AND PEMDAS

An expression combines values, variables,
and operators to produce a result.

Example:
a = 2
b = 3
c = 4

print(a + b * c)

PEMDAS:

P - Parentheses
E - Exponents
M - Multiplication
D - Division
A - Addition
S - Subtraction
""",

12: """
LESSON 12: ACCEPTING USER INPUT

The input() function allows users
to enter information.

Example:
name = input("Enter your name: ")

print("Hello,", name)

Another example:
age = input("Enter your age: ")

print("Your age is:", age)

Remember:
input() returns a string by default.
""",

13: """
LESSON 13: CONVERTING DATA TYPES

Data conversion changes one data type
into another.

int()   - Converts to integer.
float() - Converts to decimal.
str()   - Converts to string.

Example:
age = int(input("Enter age: "))
grade = float(input("Enter grade: "))

print(age)
print(grade)

Example:
number = "100"
print(int(number) + 50)

OUTPUT:
150
""",

14: """
LESSON 14: CONDITIONAL STATEMENTS

Conditional statements allow a program
to make decisions.

IF STATEMENT:

age = 18

if age >= 18:
    print("Adult")

IF-ELSE STATEMENT:

score = 85

if score >= 75:
    print("PASSED")
else:
    print("FAILED")

IF-ELIF-ELSE:

grade = 90

if grade >= 90:
    print("Excellent")
elif grade >= 75:
    print("Passed")
else:
    print("Failed")
""",

15: """
LESSON 15: RELATIONAL OPERATORS

Relational operators compare two values.

==  Equal to
!=  Not equal to
>   Greater than
<   Less than
>=  Greater than or equal
<=  Less than or equal

Example:
score = 85

print(score == 85)
print(score != 75)
print(score > 80)
print(score < 100)

The result is either True or False.
""",

16: """
LESSON 16: LOGICAL OPERATORS

Python has three logical operators.

AND:
Both conditions must be True.

OR:
At least one condition must be True.

NOT:
Reverses the condition.

Example AND:
age = 20

if age >= 18 and age <= 60:
    print("Qualified")

Example OR:
day = "Saturday"

if day == "Saturday" or day == "Sunday":
    print("Weekend")

Example NOT:
is_raining = False

if not is_raining:
    print("No rain")
""",

17: """
LESSON 17: INTRODUCTION TO ITERATION

Iteration means repeating a process.

In Python, loops repeat instructions
multiple times.

There are two main types of loops:

1. FOR LOOP
   Repeats instructions over a sequence.

2. WHILE LOOP
   Repeats instructions while a condition is True.

Example:
for number in range(1, 4):
    print("Hello Python!")
""",

18: """
LESSON 18: FOR LOOP

A for loop repeats instructions
for each item in a sequence.

Example:
for number in range(1, 6):
    print(number)

OUTPUT:
1
2
3
4
5

The loop executes the instructions
for each number in the sequence.
""",

19: """
LESSON 19: WHILE LOOP

A while loop repeats instructions
while a condition is True.

Example:
number = 1

while number <= 5:
    print(number)
    number += 1

OUTPUT:
1
2
3
4
5

The loop stops when the condition becomes False.
""",

20: """
LESSON 20: WHILE TRUE

while True creates a loop that continues
until a break statement stops it.

Example:

while True:

    name = input("Enter your name (X to exit): ")

    if name.upper() == "X":
        print("Program stopped.")
        break

    print("Hello,", name)

IMPORTANT:

while True = Repeats continuously.
break = Stops the loop.
"""
    }

    print("\n" + "=" * 55)
    print(lessons[choice])
    print("=" * 55)



print("===================================================")
print("=============== MULTIPLE CHOICE QUIZ===============")
print("===================================================")

def multiple_choice():

    questions = [
        ("What function displays output?",
         ["A. input()", "B. print()", "C. int()", "D. type()"], "B"),

        ("Which data type stores whole numbers?",
         ["A. float", "B. str", "C. int", "D. bool"], "C"),

        ("Which symbol is used for assignment?",
         ["A. ==", "B. =", "C. !=", "D. >"], "B"),

        ("What does input() do?",
         ["A. Displays output", "B. Accepts user input",
          "C. Stops a program", "D. Performs addition"], "B"),

        ("Which operator means multiplication?",
         ["A. +", "B. /", "C. *", "D. %"], "C"),

        ("What statement is used for decision-making?",
         ["A. if", "B. print", "C. input", "D. break"], "A"),

        ("Which logical operator requires both conditions True?",
         ["A. or", "B. not", "C. and", "D. if"], "C"),

        ("What loop repeats while a condition is True?",
         ["A. for", "B. while", "C. print", "D. input"], "B"),

        ("What keyword stops a loop?",
         ["A. stop", "B. exit", "C. break", "D. end"], "C"),

        ("What does Boolean store?",
         ["A. Text", "B. Decimal numbers",
          "C. True or False", "D. Whole numbers"], "C")
    ]

    score = 0

    print("\n" + "=" * 55)
    print("             MULTIPLE CHOICE QUIZ")
    print("=" * 55)

    for question, options, correct in questions:

        print("\n" + question)

        for option in options:
            print(option)

        answer = input("\nYour answer: ").upper().strip()

        if answer == correct:
            print("CORRECT!")
            score += 1
        else:
            print("INCORRECT! Correct answer:", correct)

    print("\n" + "=" * 55)
    print("              QUIZ RESULTS")
    print("=" * 55)
    print("Your Score:", score, "/", len(questions))

    if score >= 9:
        print("Excellent! Outstanding performance!")
    elif score >= 7:
        print("Very Good! Keep practicing!")
    elif score >= 5:
        print("Good effort! Review your lessons!")
    else:
        print("Keep studying! You can do better!")

    print("=" * 55)


print("===================================================")
print("================IDENTIFICATION QUIZ================")
print("===================================================")
def identification():

    questions = [
        ("What function displays information on the screen?",
         "print"),

        ("What function accepts information from the user?",
         "input"),

        ("What data type stores True or False?",
         "bool"),

        ("What keyword stops a loop?",
         "break"),

        ("What statement is used for decision-making?",
         "if")
    ]

    score = 0

    print("\n" + "=" * 55)
    print("               IDENTIFICATION QUIZ")
    print("=" * 55)

    for question, correct in questions:

        print("\n" + question)

        answer = input("Your answer: ").lower().strip()

        if answer == correct:
            print("CORRECT!")
            score += 1
        else:
            print("INCORRECT! Answer:", correct)

    print("\nYour Score:", score, "/", len(questions))

    if score >= 4:
        print("Great job! You understand the basics!")
    else:
        print("Keep reviewing your Python lessons!")

    print("=" * 55)


print("===================================================")
print("=================CODING CHALLENGE==================")
print("===================================================")

def coding_challenge():

    challenges = [
        ("Which code correctly displays Hello World?",
         ["A. print('Hello World')",
          "B. input('Hello World')",
          "C. int('Hello World')"], "A"),

        ("Which code correctly creates a variable?",
         ["A. 18 = age",
          "B. age = 18",
          "C. age == 18"], "B"),

        ("Which code correctly starts a while loop?",
         ["A. while True:",
          "B. loop True:",
          "C. repeat True:"], "A")
    ]

    score = 0

    print("\n" + "=" * 55)
    print("                CODING CHALLENGE")
    print("=" * 55)

    for question, options, correct in challenges:

        print("\n" + question)

        for option in options:
            print(option)

        answer = input("\nChoose your answer: ").upper().strip()

        if answer == correct:
            print("CORRECT!")
            score += 1
        else:
            print("INCORRECT! Correct answer:", correct)

    print("\nCODING CHALLENGE SCORE:", score, "/", len(challenges))
    print("=" * 55)


print("===================================================")
print("=====================QUIZ MENU=====================")
print("===================================================")
def quiz_menu():

    while True:

        print("\n" + "=" * 55)
        print("             PYTHON QUIZ CENTER")
        print("=" * 55)

        print("""
 [1] Multiple Choice Quiz
 [2] Identification Quiz
 [3] Coding Challenge

 [0] Back to Main Menu
 """)

        choice = input("Choose your quiz: ")

        if choice == "1":
            multiple_choice()

        elif choice == "2":
            identification()

        elif choice == "3":
            coding_challenge()

        elif choice == "0":
            break

        else:
            print("Invalid choice! Please try again.")

        input("\nPress ENTER to continue...")


print("===================================================")
print("===================MAIN PROGRAM====================")
print("===================================================")

while True:

    show_header()
    show_menu()

    choice = input("Enter your lesson number: ")

    if choice == "0":

        print("\n" + "=" * 55)
        print("=============LAST PYTHON CLDING=============")
        print("=============MAY LAST CODING HAHAHA!========")
        print("=" * 55)

        break

    elif choice.isdigit():

        choice = int(choice)

        if 1 <= choice <= 20:

            lesson(choice)

            input("\nPress ENTER to return the menu...")

        elif choice == 21:

            quiz_menu()

         
