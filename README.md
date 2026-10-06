# 90-days-placement-challenge
My 90-day placement preparation journey covering DSA, programming, projects, and interview preparation.
# 🚀 90 Days Tech Placement Preparation

I created this repository to document my progress as I learn and practice:

- C++
- Data Structures & Algorithms
- Problem Solving
- Development
- Programming Fundamentals

My goal is to build strong fundamentals, solve problems consistently, work on projects, and become better prepared for technical placements.

---

# 📅 Day 1/90 — C++ Fundamentals

Today I started my journey by learning the fundamentals of C++ and solving beginner-level programming problems.

## 📚 Topics Learned

### C++ Basics

- Basic structure of a C++ program
- `main()` function
- Compilation and execution
- Understanding the terminal/console

### Variables & Data Types

- `int`
- `double`
- `string`
- Declaring variables
- Initializing variables
- Updating variable values

### Input & Output

- `cin`
- `cout`
- `\n`
- `endl`
- Taking multiple inputs

### Arithmetic Operators

- Addition `+`
- Subtraction `-`
- Multiplication `*`
- Division `/`
- Modulo `%`

### Decision Making

- `if`
- `else`
- Comparison operators
- Understanding `=` vs `==`

### Important Concept

I also learned the difference between **integer division** and **floating-point division**.

For example:

```cpp
int a = 10;
int b = 3;

cout << a / b;



# 📅 Day 2/90 — Revision & Conditional Logic

Day 2 of my 90-day tech placement preparation journey.

Today was focused mainly on **revision, practice, and building logical thinking using conditional statements**.

I revised yesterday's C++ concepts and solved some of the previous questions again before moving on to new topics.

---

## 🔄 Revision from Day 1

I revised and practiced:

- Variables and data types
- `cin` and `cout`
- Arithmetic operators
- Modulo operator `%`
- Integer vs floating-point division
- `if/else`
- Assignment operator `=`
- Comparison operator `==`
- Beginner programming problems from Day 1

---

## 📚 New Concepts Learned

### 1. `if / else if / else`

Learned how a program can make decisions based on conditions.

```cpp
if (condition) {
    // code
}
else if (anotherCondition) {
    // code
}
else {
    // code
}
Important rule:
Conditions are checked from top to bottom, and the first true condition is executed.

2. Comparison Operators
Operator
Meaning
>
Greater than
<
Less than
>=
Greater than or equal to
<=
Less than or equal to
==
Equal to
!=
Not equal to

3. Logical Operators
AND — &&
Both conditions must be true.
if (age >= 18 && age <= 30) {
    cout << "Eligible";
}
OR — ||
At least one condition must be true.
if (day == 6 || day == 7) {
    cout << "Weekend";
}
NOT — !
Reverses a condition.
true  → false
false → true
Problems Practiced
1. Largest of Three Numbers
I created a program to find the largest among three integers.
My initial approach used the > operator:
if (a > b && a > c) {
    cout << "The largest number is: " << a;
}
While testing edge cases, I found that this approach fails when two numbers are equal.
For example:
10 10 5
The largest number is 10, but using only > would not correctly identify it in this case.
So I improved the logic using >=:
if (a >= b && a >= c) {
    cout << "The largest number is: " << a;
}
else if (b >= a && b >= c) {
    cout << "The largest number is: " << b;
}
else {
    cout << "The largest number is: " << c;
}
This handles cases where two or all three numbers are equal.
2. Leap Year
I also started working on the Leap Year problem.
The rule is:
A year divisible by 400 is a leap year.
OR, a year divisible by 4 and not divisible by 100 is a leap year.
The logical condition is:
(year % 400 == 0) || (year % 4 == 0 && year % 100 != 0)
I will continue testing this condition with different cases on Day 3.
🧠 Key Learning
Today's biggest lesson was that testing and finding edge cases is an important part of problem solving.
A solution may work for normal inputs but fail for special cases.
For example:
10 25 15 → 25
works with >.
But:
10 10 5 → 10
showed me why >= was needed.
This helped me understand that writing code is only one part of problem solving.
Thinking about different possible inputs and testing edge cases is equally important.
🎯 Day 2 Progress
[x] Revised Day 1 concepts
[x] Re-solved previous beginner problems
[x] Learned if / else if / else
[x] Learned comparison operators
[x] Learned logical operators &&, ||, !
[x] Solved largest of three numbers
[x] Tested edge cases
[x] Improved the solution using >=
[x] Started the Leap Year problem
[ ] Complete and test the Leap Year problem




---

# 📅 Day 3/90 — Conditional Logic, Problem Solving & GD Practice

Day 3 of my 90-day tech placement preparation journey.

Today I focused on strengthening my understanding of conditional logic, practicing problem-solving through decision trees, and preparing for Group Discussions.

---

## 🔄 Revision

I revised important concepts from Day 1 and Day 2, including:

- Variables and data types
- `cin` and `cout`
- Arithmetic operators
- Modulo operator `%`
- Comparison operators
- `if / else if / else`
- Logical operators `&&`, `||`, `!`
- Edge cases
- Dry runs

I also briefly reviewed `switch` statements, but since I had already studied the topic, I focused my time on problem solving instead.

---

## 📚 Concepts Practiced

### 1. Leap Year Logic

I completed the Leap Year problem and tested it with important edge cases.

The condition I used was:

```cpp
(year % 400 == 0) || (year % 4 == 0 && year % 100 != 0)
I tested:
2024 → Leap Year
1900 → Not a Leap Year
2000 → Leap Year
This helped me understand why simply checking whether a year is divisible by 4 is not enough.

2. Nested if Statements
I learned how to place one if statement inside another if statement.
Example structure:
if (condition1) {

    if (condition2) {
        // code
    }
    else {
        // code
    }

}
else {
    // code
}
The important idea I learned is:
The inner decision can depend on the outer decision.
For example, when checking whether someone can enter:
Is the person 18 or older?
        |
        YES
        |
    Check ID
      /   \
    YES   NO
    |      |
  Allow   Need ID
This helped me understand how to build a decision tree before writing the actual code.
🧠 Problem Solving Practice
I worked on a number classification problem.
The goal was to determine whether a number is:
Positive Even
Positive Odd
Negative Even
Negative Odd
Zero
The decision-making approach was:
              n == 0?
             /       \
          YES         NO
          |           |
        Zero        n > 0?
                    /     \
                  YES      NO
                   |        |
              Positive   Negative
                 |          |
              Even/Odd    Even/Odd
This problem helped me practice combining:
if / else if / else
Nested if
Comparison operators
Modulo %
Logical reasoning
Decision trees
I also learned that zero should be handled separately before checking whether the number is positive or negative.
🧪 Edge Cases & Dry Runs
Today I continued practicing dry runs instead of immediately executing code.
Some important cases I considered were:
18 → boundary case for adulthood
0  → special case for number classification
1900 → leap year edge case
2000 → leap year edge case
This reinforced an important lesson:
A solution should not only work for normal inputs. It should also handle boundary cases and special cases correctly.
🎤 Group Discussion Preparation
Along with technical preparation, I also spent time preparing for Group Discussions.
I participated in a GD with my friends through Google Meet.
During the session, I practiced:
Expressing my thoughts clearly
Speaking with confidence
Listening to other participants
Understanding different viewpoints
Responding to others' opinions
Maintaining a structured flow while speaking
This gave me practical experience instead of only preparing theoretically.
I realized that placement preparation requires more than technical knowledge.
Technical skills + problem solving + communication + confidence all matter.
🧠 Key Learnings
Today's biggest lessons were:
Think about the decision structure before writing code.
Use nested conditions when one decision depends on another.
Always consider edge cases.
Dry-run the logic before executing the program.
Communication skills are also an important part of placement preparation.
🎯 Day 3 Progress
[x] Revised Day 1 and Day 2 concepts
[x] Completed Leap Year logic
[x] Tested Leap Year edge cases
[x] Learned and practiced nested if
[x] Practiced decision trees
[x] Practiced dry runs
[x] Started number classification problem
[x] Prepared for Group Discussion
[x] Participated in a GD with friends through Google Meet
[x] Complete final testing of the number classification problem
🚀 Day 3/90
Think → Plan → Code → Test → Find edge cases → Improve.
Day 3/90 — Almost Complete ✅