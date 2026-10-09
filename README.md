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





# Day 04 — Revision, Loops & Placement Preparation

## 📚 Topics Covered

Today was a lighter study day focused mainly on revision and maintaining consistency.

### C++ Revision
- Revised concepts learned during previous days
- Reviewed conditional statements
- Reviewed nested `if`
- Reviewed logical and comparison operators
- Reviewed edge cases and dry runs

### Number Classification

Completed and tested the number classification problem.

The program classifies a number as:

- Positive Even
- Positive Odd
- Negative Even
- Negative Odd
- Zero

### Loops — Introduction

Started learning the fundamentals of loops.

Understood the three important parts of a loop:

1. Initialization
2. Condition
3. Update

Example concept:

```cpp
int i = 1;
Condition:
i <= 5
Update:
i = i + 1;
Understood why:
i <= 5
allows values from 1 through 5, while:
i == 5
is only true when i is exactly 5.
🗣️ Group Discussion Practice
Participated in another Group Discussion with friends through Google Meet.
Skills Practiced
Communication
Confidence
Active listening
Expressing ideas clearly
Responding to different viewpoints
Participating in discussions
Regular GD practice is helping me prepare not only technically but also for the communication and discussion rounds of placements.
🧠 Key Learnings
Revision is important for retaining previously learned concepts.
Understanding the logic behind loops is more important than memorizing syntax.
Conditions determine when a loop continues or stops.
Consistency matters even on low-energy days.
Placement preparation requires both technical and communication skills.
✅ Day 04 Checklist
[x] Revise previous C++ concepts
[x] Complete number classification problem
[x] Test positive, negative, even, odd and zero cases
[x] Understand basic loop structure
[x] Understand initialization, condition and update
[x] Participate in Group Discussion
[x] Practice communication skills
[ ] Complete for loop syntax and practice
[ ] Start Time & Space Complexity
💡 Day 04 Takeaway
Consistency doesn't mean every day has to be perfect.
The goal is to keep moving forward.


---

# Day 05 — Group Discussion & Placement Preparation

## Activities

Day 5 was a lighter day focused on placement preparation outside technical coding.

### Group Discussion Practice

Participated in a Group Discussion with friends through Google Meet.

### Skills Practiced
- Communication
- Active listening
- Expressing ideas clearly
- Building confidence
- Understanding different viewpoints
- Responding thoughtfully during discussions

## Key Learnings

- Technical knowledge is only one part of placement preparation.
- Communication and teamwork are also important.
- Consistency matters more than having a perfect study schedule every day.

## Day 5 Checklist

- [x] Participate in Group Discussion
- [x] Practice communication skills
- [ ] C++ coding practice
- [ ] DSA practice

## Reflection

Although I did not complete a coding session today, I continued working on my placement preparation through communication practice.

The goal is to keep improving throughout the 90-day journey.





# Day 06 — Loops, Typecasting & Revision

## 📚 Topics Covered

### 1. Loops in C++

Completed the topic of loops in C++ and practiced the concepts through examples and code.

Topics covered:
- `for` loop
- `while` loop
- `do-while` loop
- Loop initialization, condition, and update
- Controlling loop execution
- Practicing repetition through loops

### 2. Typecasting in C++

Learned about type conversion and its role in C++ programming.

#### Implicit Typecasting

Implicit typecasting occurs when the compiler automatically converts a value from one data type to another in certain situations.

Example:

```cpp
#include <iostream>
using namespace std;

int main() {
    int num = 10;
    double result = num;

    cout << result;

    return 0;
}
Output:
10
Here, the integer value is converted to a double automatically.
Explicit Typecasting
Explicit typecasting occurs when the programmer explicitly requests a conversion.
Example:
#include <iostream>
using namespace std;

int main() {
    double num = 9.75;
    int result = static_cast<int>(num);

    cout << result;

    return 0;
}
Output:
9
Here, static_cast<int>(num) explicitly converts the double value to an int. The fractional part is discarded.
3. Revision
Reviewed previous notes.
Strengthened understanding of previously learned C++ concepts.
Practiced writing code to reinforce theoretical knowledge.
🧠 Key Learnings
Loops allow repetitive tasks to be performed efficiently.
Implicit typecasting is performed automatically by the compiler in appropriate contexts.
Explicit typecasting allows the programmer to request a specific conversion.
Converting from a floating-point type to an integer discards the fractional part; it does not round to the nearest integer.
Regular revision helps reinforce previously learned concepts.
✅ Day 06 Checklist
[x] Complete loops in C++
[x] Learn implicit typecasting
[x] Learn explicit typecasting
[x] Practice typecasting with code examples
[x] Review previous notes
💡 Day 06 Takeaway
Learn the concept, understand the behavior, write the code, and practice until the logic becomes clear.