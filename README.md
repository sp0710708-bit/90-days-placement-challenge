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




---

# Day 07 — Functions in C++ & Group Discussion

## 💻 Topics Covered

### 1. Introduction to Functions

Started learning about functions in C++.

Functions help divide a program into smaller, reusable blocks of code. They make programs easier to organize, understand, test, and maintain.

### 2. Void Functions

Learned about `void` functions in C++.

A `void` function performs a task but does not return a value to its caller.

Example:

```cpp
#include <iostream>
using namespace std;

void greet() {
    cout << "Hello, welcome to C++!";
}

int main() {
    greet();
    return 0;
}
```

**Output:**

```text
Hello, welcome to C++!
```

In this example:
- `void` indicates that the function does not return a value.
- `greet()` is the function name.
- The function body contains the task to perform.
- `greet();` calls the function from `main()`.

## 🗣️ Placement Preparation — Group Discussion

Participated in another Group Discussion with friends through Google Meet.

### Skills Practiced

- Communication
- Active listening
- Expressing ideas clearly
- Confidence while speaking
- Responding to different viewpoints

Regular Group Discussion practice is helping me work on the communication skills required for placement preparation.

## 🧠 Key Learnings

- Functions help organize programs into reusable blocks.
- A `void` function does not return a value.
- Functions can be called whenever their behavior is needed.
- Technical knowledge and communication skills are both important for placement preparation.

## ✅ Day 07 Checklist

- [x] Begin learning functions in C++
- [x] Understand the basic concept of `void` functions
- [x] Practice a basic void function
- [x] Participate in Group Discussion
- [x] Practice communication skills
- [ ] Continue learning function parameters and return values
- [ ] Practice more function-based problems

## 💡 Day 07 Takeaway

> Consistent learning, practical coding, and communication practice are all part of becoming placement-ready.





---

# Day 08 — C++ Revision, Function Anatomy & GD Practice

## 📚 Topics Covered

### 1. Revision of Previous Concepts

Revisited previously learned C++ concepts and practiced earlier problems.

**Goal:**
- Strengthen fundamental concepts.
- Improve retention through revision.
- Identify areas that need additional practice.

### 2. Functions in C++

Continued learning about functions in C++.

#### Function Anatomy

Studied the basic structure and components of a function.

Example:

```cpp
#include <iostream>
using namespace std;

void greet() {
    cout << "Hello!";
}

int main() {
    greet();
    return 0;
}
```

**Output:**

```text
Hello!
```

#### Components of a Function

- `void` — return type; indicates that the function does not return a value.
- `greet` — function name.
- `()` — parentheses containing parameters, if any.
- `{}` — function body containing the statements to execute.
- `greet();` — function call that executes the function.

### 3. Group Discussion Practice

Participated in another Group Discussion practice session with friends.

**Skills practiced:**
- Communication
- Active listening
- Expressing ideas clearly
- Building confidence
- Responding to different viewpoints

## 🧠 Key Learnings

- Revision helps reinforce previously learned concepts.
- Understanding function structure is important for writing organized C++ programs.
- Functions help divide programs into smaller, reusable units.
- Technical preparation and communication practice are both important for placement readiness.
- Consistent effort matters, even on slower days.

## ✅ Day 08 Checklist

- [x] Revise previously learned C++ concepts
- [x] Practice previous problems
- [x] Continue studying functions
- [x] Study function anatomy
- [x] Participate in Group Discussion practice
- [ ] Continue learning function parameters and return values
- [ ] Solve additional function-based problems

## 💡 Day 08 Reflection

Today was a lighter study day, but I continued working on my technical fundamentals and communication skills.

My next goal is to improve my time management, practice more independently, and keep progressing toward DSA.

> Progress is not always fast, but every honest effort can contribute to long-term improvement.




## Day 9 – Loop Control and Nested Loops

### 📚 Topics Practiced
- Reviewed `for`, `while`, and `do-while` loops.
- Practiced the `break` statement to terminate a loop.
- Practiced the `continue` statement to skip an iteration.
- Started learning nested loops.
- Practiced tracing code execution and predicting outputs.
- Participated in Group Discussion (GD) practice with friends.

### 💡 Key Learnings
- `break` immediately terminates the loop.
- `continue` skips the current iteration and proceeds to the next one.
- A nested loop is a loop inside another loop.
- The inner loop completes its iterations for each iteration of the outer loop.
- The position of statements such as `cout << endl;` affects the output format.

### 🧠 Practice and Reflection
I practiced several loop-based examples and worked on understanding
how the values of loop variables change during execution.

Nested loops are a concept I need to practice further, especially
understanding the relationship between the inner and outer loops.

I also practiced Group Discussion with friends to improve my
communication and confidence for placement preparation.

### 🎯 Next Steps
- Continue practicing nested loops.
- Improve my ability to trace loop execution step by step.
- Solve more beginner-level C++ exercises.
- Continue regular GD practice.

**Progress:** Continued strengthening C++ fundamentals and
identified nested loops as an area for further practice.




## Day 10 - C++ Practice

### Topics Learned and Practiced
- Revised loops in C++.
- Practiced nested loops and understood the relationship between outer and inner loops.
- Explored basic pattern printing using nested loops.
- Learned more about functions in C++.
- Wrote function code independently to improve my understanding and coding skills.

### Key Takeaways
- Loops help automate repetitive tasks.
- Nested loops can be used to work with rows, columns, and patterns.
- Functions help organize code into reusable blocks.
- Writing code independently helps strengthen logical thinking and problem-solving skills.

### Reflection
Today, I focused on strengthening my understanding of loops and functions.
I practiced nested loops and explored basic patterns. I also wrote function
code by myself, which helped me gain more confidence in applying what I learned.

I will continue practicing these concepts to improve my understanding and coding skills.

**Status:** Day 10 completed.




## Day 11 - Revision, Debugging, and GD Practice

### Activities Completed
- Worked on debugging C++ programming problems.
- Revised previously learned C++ concepts.
- Practiced identifying and correcting errors in code.
- Participated in Group Discussion (GD) practice to improve communication skills.

### Key Takeaways
- Debugging helps identify mistakes and improve code correctness.
- Regular revision strengthens understanding and retention.
- Consistent practice helps build confidence in programming.
- Group Discussions help develop communication and idea-expression skills.

### Reflection
Today, I focused on revising previous topics and debugging programming
problems instead of rushing into new concepts. I also practiced Group
Discussions as part of my overall placement preparation.

I will continue strengthening my fundamentals through regular revision,
hands-on coding, and communication practice.

**Status:** Day 11 completed.





## Day 12 - C++ Data Types and Computer Fundamentals

### Topics Learned
- Studied C++ data types and their purpose.
- Learned the differences between signed and unsigned integers.
- Explored how positive and negative integers are represented in memory.
- Studied the differences between 32-bit and 64-bit architectures.
- Revised previously learned C++ concepts.
- Practiced Group Discussions (GD) to improve communication skills.

### Key Takeaways
- Data types determine the kind of values a variable can represent.
- Signed integer types can represent negative and positive values, while unsigned integer types represent non-negative values.
- Computers use binary representations to store numerical data.
- 32-bit and 64-bit architectures differ in important ways, including their address-space capabilities.
- Regular revision helps reinforce programming fundamentals.
- GD practice supports communication and confidence development.

### Reflection
Today, I explored C++ data types, signed and unsigned integers, number
representation in memory, and the differences between 32-bit and 64-bit
architectures. I also revised previous topics and practiced GD.

My goal is to understand not only how to write code, but also how computers
represent and process the data used by that code.

I will continue strengthening my fundamentals through revision and consistent practice.

**Status:** Day 12 completed.




## Day 13 — Algorithms and Flowcharts

### Topics Covered
- Introduction to algorithms
- Importance and characteristics of algorithms
- Introduction to flowcharts
- Flowchart components and symbols
- Representing problem-solving logic visually

### Practical Work
- Designed multiple flowcharts to understand program logic.
- Practiced identifying the appropriate flowchart symbols for different operations.
- Worked on organizing problem-solving steps before implementation.

### Communication Practice
- Continued daily Group Discussion (GD) practice.
- Focused on improving communication, confidence, and idea organization.

### Key Takeaway
Algorithms provide step-by-step instructions for solving problems, while flowcharts represent those steps visually. Planning the logic before coding helps make solutions clearer and easier to implement.

### Progress
- [x] Studied algorithms
- [x] Learned flowchart components
- [x] Designed multiple flowcharts
- [x] Practiced Group Discussion

**Day 13 completed — continuing the 90 Days Placement Preparation Challenge!**





## Day 14 — Revision and GD Practice

### Today's Activities
- Revised notes from previously studied topics.
- Reviewed programming fundamentals to reinforce understanding.
- Practiced Group Discussions (GD).

### Key Takeaways
- Regular revision helps strengthen conceptual understanding.
- Revisiting previous topics helps identify gaps in knowledge.
- GD practice supports communication, confidence, and structured thinking.
- Consistency is essential for long-term placement preparation.

### Progress Checklist
- [x] Revised notes
- [x] Reviewed previous concepts
- [x] Practiced Group Discussions

**Day 14 completed — 14 days of consistent placement preparation!**



## Day 15 — Preparation and Planning

### Today's Focus
- Reviewed current priorities and upcoming goals.
- Organized my next steps for continued placement preparation.
- Reflected on the importance of consistency, adaptability, and time management.

### Key Takeaways
- Progress isn't always measured by the number of topics completed.
- Managing priorities is an important professional skill.
- Consistency means continuing the journey, even when daily schedules change.

### Progress Checklist
- [x] Reviewed priorities
- [x] Reflected on placement preparation goals
- [x] Planned the next steps

**Day 15 completed — staying committed to the 90 Days Placement Preparation Challenge.**




## 📅 Days 16–17: Reflection & Staying Consistent 🌱

The past two days were a reminder that a learning journey doesn't always go according to plan.

Although I couldn't make as much technical progress as I had planned, I remained committed to my 90-day placement preparation challenge.

### 💡 Key Takeaways
- Consistency is about returning to your goals, even after a pause.
- Time management is an important part of placement preparation.
- Progress is not always measured by the amount of code written.
- Staying committed matters more than being perfect every day.

### 🎯 Moving Forward
I'll continue strengthening my C++ fundamentals, practising problem-solving, and documenting my actual learning and code on GitHub.

**The journey continues — one step at a time! 🚀**



## Day 18 — Placement Preparation and GD Practice

### Today's Activities
- Attended a company pre-placement presentation (PPT).
- Participated in a Group Discussion (GD).
- Observed the importance of communication and teamwork in recruitment.

### Key Takeaways
- Clear communication is essential during group discussions.
- Active listening and structured thinking improve participation.
- Understanding the recruitment process helps with career preparation.

### Progress Checklist
- [x] Attended company PPT
- [x] Participated in GD
- [x] Reflected on communication and professional skills

**Day 18 completed — continuing the 90 Days Placement Preparation Challenge!**




## Day 19 — Revision and GD Practice

### Today's Focus
- Revised notes from previously studied technical topics.
- Reinforced understanding of programming fundamentals.
- Practiced Group Discussions (GD).

### Key Takeaways
- Revision strengthens conceptual understanding.
- Regular practice helps identify knowledge gaps.
- GD practice improves communication, confidence, and structured thinking.

### Progress Checklist
- [x] Revised previous notes
- [x] Reviewed technical concepts
- [x] Practiced Group Discussions

**Day 19 completed — continuing the 90 Days Placement Preparation Challenge!**
