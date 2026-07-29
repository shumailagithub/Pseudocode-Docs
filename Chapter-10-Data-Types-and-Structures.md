📚 Cambridge International AS & A Level Computer Science (9618)

Chapter 10 – Data Types and Structures

├── Learning Objectives
├── Introduction
├── Real-life analogy
├── Every concept explained in simple English
├── Teacher Notes (what to tell students)
├── Cambridge Exam Notes
├── Diagrams using Markdown
├── Tables
├── Easy Examples
├── Real-world Examples
├── Step-by-step Pseudocode
├── Dry Run Examples
├── Bubble Sort Animation (ASCII)
├── Linear Search Walkthrough
├── Arrays Explained Visually
├── Records Explained Visually
├── Files Explained
├── Stack Explained
├── Queue Explained
├── Linked List Explained
├── ADT Comparison Table
├── Common Student Mistakes
├── Exam Questions
├── MCQs
├── Long Questions
├── Practical Exercises
├── Homework
└── Revision Summary





# INTEGER Data Type

## What is an INTEGER?

An INTEGER stores whole numbers only. It cannot store decimal values.

Examples:

- 5
- 20
- -100

Real-life Example

Imagine a classroom.

Number of students = 32

Since there cannot be 32.5 students, INTEGER is the correct data type.

---

## Cambridge Pseudocode

```text
DECLARE Age : INTEGER

Age ← 18
```

---

## Explanation

Here,

Age is the variable.

INTEGER tells the computer that Age can only store whole numbers.

18 is assigned to Age.

---

## Memory Representation

Age

+-------+
|  18   |
+-------+

---

## Common Mistakes

❌ Age ← 18.5

This is incorrect because INTEGER cannot store decimal values.

Use REAL instead.

---




# Chapter 10 - Data Types and Structures
**Cambridge International AS & A Level Computer Science (9618)**

---

# Table of Contents

1. Introduction
2. Learning Objectives
3. Data Types
4. Choosing the Correct Data Type
5. Records
6. Arrays
7. Array Terminology
8. One-Dimensional Arrays
9. Two-Dimensional Arrays

---

# Introduction

Imagine you are developing a **School Management System**.

The system needs to store:

- Student Name
- Student Age
- Student Marks
- Student Date of Birth
- Attendance
- Examination Results

A computer cannot simply store everything in the same way.

For example,

- Age is a number.
- Name is text.
- Date of Birth is a date.
- Pass/Fail is either TRUE or FALSE.

Therefore, programmers use **Data Types** to tell the computer what kind of data is being stored.

Sometimes we also need to store many values together. For this, we use **Records** and **Arrays**.

This chapter teaches you how to organise data efficiently.

---

# Learning Objectives

After completing this chapter, you should be able to:

- Select the correct data type.
- Explain the purpose of records.
- Create records in pseudocode.
- Read from and write to records.
- Create one-dimensional arrays.
- Create two-dimensional arrays.
- Understand array terminology.
- Process array data.

---

# 10.1 Data Types

## What is a Data Type?

A **data type** tells the computer what kind of information a variable will store.

Think of it like different storage boxes.

Imagine you are packing items into boxes.

```
Books → Book Box

Clothes → Clothes Box

Shoes → Shoe Box
```

You would never place shoes inside a book box.

Similarly,

- Numbers go into numeric variables.
- Text goes into string variables.
- TRUE/FALSE goes into Boolean variables.

Choosing the correct data type helps:

- Save memory
- Prevent errors
- Improve program efficiency
- Make programs easier to understand

---

# Cambridge Data Types

| Data Type | Stores | Example |
|------------|---------|----------|
| INTEGER | Whole numbers | 25 |
| REAL | Decimal numbers | 18.75 |
| CHAR | One character | 'A' |
| STRING | Multiple characters | "Ahmed" |
| BOOLEAN | TRUE or FALSE | TRUE |
| DATE | Dates | 15/07/2026 |
| ARRAY | Multiple values of same type | Marks[1..30] |
| FILE | Permanent data storage | Students.txt |

---

# INTEGER

## Definition

INTEGER stores **whole numbers only**.

It cannot store decimal numbers.

Examples

```
10
55
-8
0
250
```

Examples that are NOT integers

```
12.5
3.14
99.99
```

---

## Real Life Example

Student Age

```
Age = 17
```

Age is always stored as INTEGER because it is a whole number.

---

## Cambridge Pseudocode

```text
DECLARE Age : INTEGER

Age ← 17
```

Explanation

```
DECLARE

Creates a variable.

Age

Variable name.

INTEGER

Specifies that Age stores whole numbers.

←

Assignment operator.

17

Value assigned.
```

---

## Memory Representation

```
Age

+------+
|  17  |
+------+
```

---

## Common Mistakes

Incorrect

```text
DECLARE Age : INTEGER

Age ← 17.5
```

Why?

17.5 contains a decimal.

Correct data type should be REAL.

---

# REAL

## Definition

REAL stores decimal numbers.

Examples

```
1.5

98.75

3.14159

-2.7
```

---

## Real Life Example

Height

```
1.72 metres
```

Temperature

```
36.8°C
```

Weight

```
68.5 kg
```

All require REAL because they contain decimal values.

---

## Cambridge Pseudocode

```text
DECLARE Height : REAL

Height ← 1.72
```

---

## Memory Representation

```
Height

+--------+
| 1.72   |
+--------+
```

---

# CHAR

## Definition

CHAR stores exactly **one character**.

Examples

```
'A'

'7'

'@'

'B'
```

Notice the single quotation marks.

---

## Real Life Example

Student Grade

```
A

B

C

D
```

Only one letter is stored.

---

## Cambridge Pseudocode

```text
DECLARE Grade : CHAR

Grade ← 'A'
```

---

## Common Mistake

Incorrect

```text
Grade ← 'AB'
```

Why?

CHAR stores only ONE character.

---

# STRING

## Definition

STRING stores text consisting of multiple characters.

Examples

```
Ali

Pakistan

Computer Science

Cambridge
```

---

## Real Life Example

Student Name

```
Ahmed Khan
```

City

```
Karachi
```

School Name

```
The City School
```

---

## Cambridge Pseudocode

```text
DECLARE Name : STRING

Name ← "Ali"
```

---

## Difference between CHAR and STRING

| CHAR | STRING |
|-------|---------|
| One character | Many characters |
| 'A' | "Ahmed" |
| '7' | "12345" |

---

# BOOLEAN

## Definition

BOOLEAN stores only two values.

```
TRUE

FALSE
```

---

## Real Life Example

Has student paid fees?

```
TRUE
```

Is exam passed?

```
FALSE
```

Is door locked?

```
TRUE
```

---

## Cambridge Pseudocode

```text
DECLARE Passed : BOOLEAN

Passed ← TRUE
```

---

## Used in Decision Making

```text
IF Passed = TRUE THEN

    OUTPUT "Congratulations"

ENDIF
```

---

# DATE

## Definition

DATE stores dates.

Examples

```
20/04/2026

01/01/2027

15/08/2025
```

---

## Real Life Example

Date of Birth

Admission Date

Exam Date

Appointment Date

---

## Cambridge Pseudocode

```text
DECLARE DOB : DATE
```

---

# ARRAY Data Type

An ARRAY stores multiple values of the **same data type**.

Example

Instead of creating

```text
Mark1

Mark2

Mark3

Mark4

Mark5
```

We create

```text
Marks[1]

Marks[2]

Marks[3]

Marks[4]

Marks[5]
```

This makes programs shorter and easier to manage.

---

# FILE Data Type

A FILE stores data permanently.

Variables lose data when the program closes.

Files keep data even after the program ends.

Example

```
Students.txt

Employees.txt

Marks.txt
```

---

# Choosing the Correct Data Type

This is a favourite Cambridge examination question.

Choose the most appropriate data type.

| Information | Data Type |
|--------------|------------|
| Student Name | STRING |
| Student Age | INTEGER |
| Exam Percentage | REAL |
| Grade | CHAR |
| Date of Birth | DATE |
| Passed | BOOLEAN |

---

# Classroom Activity

Ask students

Choose the correct datatype.

```
Number of books

Student name

Temperature

Date of Birth

Gender (M/F)

Exam Result
```

Answers

```
INTEGER

STRING

REAL

DATE

CHAR

BOOLEAN
```

---

# 10.1 Records

## What is a Record?

A **Record** is a collection of related data stored under one name.

Unlike an array, a record can store **different data types together**.

Think about a student.

A student has

- Name
- Age
- Date of Birth
- Marks
- Passed

These are different types of information.

Instead of creating many separate variables, we group them together.

---

## Real Life Example

```
Student

├── Name

├── Age

├── DOB

├── Marks

└── Passed
```

Everything belongs to one student.

---

# Why Do We Need Records?

Without Records

```text
Name

Age

Marks

DOB

Passed
```

Many separate variables.

With Records

```text
Student.Name

Student.Age

Student.DOB

Student.Marks

Student.Passed
```

Everything stays organised.

---

# Defining a Record

Cambridge pseudocode

```text
TYPE StudentRecord

    DECLARE Name : STRING

    DECLARE Age : INTEGER

    DECLARE DOB : DATE

    DECLARE Marks : REAL

    DECLARE Passed : BOOLEAN

ENDTYPE
```

---

# Creating a Record Variable

```text
DECLARE Student : StudentRecord
```

---

# Saving Data into a Record

```text
Student.Name ← "Ali"

Student.Age ← 17

Student.DOB ← 15/06/2009

Student.Marks ← 86.5

Student.Passed ← TRUE
```

---

# Reading Data from a Record

```text
OUTPUT Student.Name

OUTPUT Student.Age

OUTPUT Student.Marks

OUTPUT Student.Passed
```

---

# Record vs Array

| Record | Array |
|----------|--------|
| Different data types | Same data type |
| Stores one object's details | Stores many similar values |
| Student record | Student marks |

Example

Record

```
Student

Name

Age

Marks

Passed
```

Array

```
Marks

85

90

77

68

95
```

---

# 10.2 Arrays

## What is an Array?

An array stores multiple values of the same data type under one variable name.

Without arrays

```text
Score1

Score2

Score3

Score4

Score5
```

With arrays

```text
Scores[1]

Scores[2]

Scores[3]

Scores[4]

Scores[5]
```

Arrays reduce code repetition and make processing easier.

---

# Advantages of Arrays

- Less code
- Easier processing
- Easy searching
- Easy sorting
- Saves programming time

---

# Array Terminology

## Index

The position number of an element.

Example

```
Marks

Index

1 → 80

2 → 72

3 → 95

4 → 60

5 → 88
```

Index tells us where data is stored.

---

# Lower Bound

The first valid index.

Example

```text
DECLARE Marks : ARRAY[1:5] OF INTEGER
```

Lower Bound = 1

---

# Upper Bound

The last valid index.

Example

```text
DECLARE Marks : ARRAY[1:5] OF INTEGER
```

Upper Bound = 5

---

# Accessing an Array Element

```text
OUTPUT Marks[3]
```

Output

```
95
```

because element number 3 contains 95.

---

# One-Dimensional Array (1D Array)

A one-dimensional array is like a single row of lockers.

```
Index

1

2

3

4

5
```

Each locker stores one value.

---

# Declaring a 1D Array

```text
DECLARE Marks : ARRAY[1:5] OF INTEGER
```

---

# Input Values into a 1D Array

```text
FOR i ← 1 TO 5

    INPUT Marks[i]

NEXT i
```

Explanation

The loop asks the user to enter five values.

Each value is stored in the next array position.

---

# Display Array Values

```text
FOR i ← 1 TO 5

    OUTPUT Marks[i]

NEXT i
```

---

# Visual Representation

```
Index

1   2   3   4   5

+---+---+---+---+---+

85  72  90  68  95

+---+---+---+---+---+
```

---

# Two-Dimensional Array (2D Array)

A two-dimensional array stores data in rows and columns.

Think of an Excel spreadsheet.

```
        Maths English Science

Ali      80      75      90

Sara     95      88      92

Ahmed    70      82      79
```

A 2D array is ideal for storing tabular data.

---

# Declaring a 2D Array

```text
DECLARE Marks : ARRAY[1:3,1:3] OF INTEGER
```

The first number represents rows.

The second number represents columns.

---

# Accessing Values

```text
OUTPUT Marks[2,3]
```

This means:

Row = 2

Column = 3

---

# End of Part 1

In **Part 2**, we will cover:

- Processing Arrays
- Finding Total, Average, Maximum and Minimum
- Bubble Sort (step-by-step dry run)
- Linear Search (step-by-step dry run)
- Files (complete explanation)
- Abstract Data Types (ADT)
- Stack (LIFO)
- Queue (FIFO)
- Linked List
- ADT Implementation using Arrays
- Cambridge Exam Tips
- Common Mistakes
- MCQs
- Practical Exercises
- Homework
- Revision Summary






---

# 10.2 Processing Arrays

Creating an array is only the first step. In real programs, we usually need to **process** the data stored inside the array.

Processing means performing operations such as:

- Reading values
- Displaying values
- Finding the total
- Finding the average
- Finding the highest value
- Finding the lowest value
- Searching
- Sorting

---

# Reading Values into an Array

Suppose a teacher wants to enter marks for five students.

Instead of writing:

```text
INPUT Mark1
INPUT Mark2
INPUT Mark3
INPUT Mark4
INPUT Mark5
```

we use a loop.

```text
DECLARE Marks : ARRAY[1:5] OF INTEGER

FOR i ← 1 TO 5
    INPUT Marks[i]
NEXT i
```

## Explanation

Initially

```
Marks

Index

1
2
3
4
5
```

Suppose the teacher enters

```
85
70
92
61
88
```

The array becomes

```
Index

1 → 85

2 → 70

3 → 92

4 → 61

5 → 88
```

The loop automatically stores every value in the next array position.

---

# Displaying Array Values

```text
FOR i ← 1 TO 5
    OUTPUT Marks[i]
NEXT i
```

Output

```
85

70

92

61

88
```

---

# Finding the Total

Suppose we want to calculate the total marks.

Example

```
85

70

92

61

88
```

Total

```
396
```

---

## Algorithm

Step 1

Create a variable called Total.

```
Total ← 0
```

Step 2

Visit every array element.

Step 3

Add each value to Total.

---

## Cambridge Pseudocode

```text
DECLARE Total : INTEGER

Total ← 0

FOR i ← 1 TO 5

    Total ← Total + Marks[i]

NEXT i

OUTPUT Total
```

---

## Dry Run

Initial

```
Total = 0
```

After reading 85

```
Total = 85
```

After reading 70

```
Total = 155
```

After reading 92

```
Total = 247
```

After reading 61

```
Total = 308
```

After reading 88

```
Total = 396
```

---

# Finding the Average

Formula

```
Average = Total ÷ Number of Values
```

Example

```
Total = 396

Students = 5

Average = 396 / 5

Average = 79.2
```

---

## Cambridge Pseudocode

```text
Average ← Total / 5

OUTPUT Average
```

---

# Finding the Maximum Value

The maximum value is the largest number.

Example

```
85

70

92

61

88
```

Maximum

```
92
```

---

## Algorithm

Assume the first value is the largest.

Compare it with every other value.

Whenever a larger value is found, replace Maximum.

---

## Cambridge Pseudocode

```text
Maximum ← Marks[1]

FOR i ← 2 TO 5

    IF Marks[i] > Maximum THEN

        Maximum ← Marks[i]

    ENDIF

NEXT i

OUTPUT Maximum
```

---

## Dry Run

```
Maximum = 85

Compare 70

Still 85

Compare 92

Maximum becomes 92

Compare 61

Still 92

Compare 88

Still 92
```

---

# Finding the Minimum Value

Minimum means the smallest value.

Example

```
85

70

92

61

88
```

Minimum

```
61
```

---

## Cambridge Pseudocode

```text
Minimum ← Marks[1]

FOR i ← 2 TO 5

    IF Marks[i] < Minimum THEN

        Minimum ← Marks[i]

    ENDIF

NEXT i

OUTPUT Minimum
```

---

# Bubble Sort

Bubble Sort is one of the easiest sorting algorithms.

It repeatedly compares **two neighbouring values**.

If they are in the wrong order, they are swapped.

This process repeats until the entire array becomes sorted.

---

## Real-Life Example

Imagine children standing according to height.

```
Tall

Short

Medium

Very Tall
```

The teacher compares neighbouring children and swaps them until everyone is standing in order.

Bubble Sort works in exactly the same way.

---

# Example

Original Array

```
45

20

60

10
```

---

## Pass 1

Compare

```
45

20
```

45 > 20

Swap

```
20

45

60

10
```

---

Compare

```
45

60
```

Correct order

No swap.

---

Compare

```
60

10
```

Swap

```
20

45

10

60
```

---

## Pass 2

Compare

```
20

45
```

Correct.

Compare

```
45

10
```

Swap.

```
20

10

45

60
```

---

## Pass 3

Compare

```
20

10
```

Swap.

```
10

20

45

60
```

Array Sorted

---

# Bubble Sort Pseudocode

```text
FOR Pass ← 1 TO 3

    FOR i ← 1 TO 3

        IF Marks[i] > Marks[i+1] THEN

            Temp ← Marks[i]

            Marks[i] ← Marks[i+1]

            Marks[i+1] ← Temp

        ENDIF

    NEXT i

NEXT Pass
```

---

# Why is it called Bubble Sort?

The largest value slowly moves towards the end of the array, just like an air bubble rises to the top of water.

---

# Linear Search

Linear Search checks every element one by one until the required value is found.

---

## Example

Array

```
10

25

30

48

90
```

Search

```
48
```

Process

```
10

Not found

↓

25

Not found

↓

30

Not found

↓

48

Found
```

---

# Cambridge Pseudocode

```text
Found ← FALSE

FOR i ← 1 TO 5

    IF Marks[i] = SearchValue THEN

        Found ← TRUE

        OUTPUT "Found"

    ENDIF

NEXT i
```

---

# Advantages of Linear Search

- Easy to understand.
- Easy to program.
- Works with unsorted arrays.

---

# Disadvantages

- Slow for large arrays.
- Checks every element.

---

# 10.3 Files

## What is a File?

A file stores data permanently.

Variables lose their values when the program ends.

Files keep information even after the computer is switched off.

---

## Why Do We Need Files?

Suppose a school stores:

- Student names
- Marks
- Attendance
- Teachers

If all this data were stored in variables, everything would disappear after the program closed.

Files solve this problem.

---

# Types of Files

Cambridge Paper 2 mainly focuses on **Text Files**.

Example

```
Students.txt

Marks.txt

Names.txt
```

---

# Opening a File

Before using a file, it must be opened.

```text
OPENFILE "Students.txt" FOR READ
```

---

# Reading a File

```text
OPENFILE "Students.txt" FOR READ

READFILE "Students.txt", Name

OUTPUT Name

CLOSEFILE "Students.txt"
```

---

# Writing to a File

```text
OPENFILE "Students.txt" FOR WRITE

WRITEFILE "Students.txt", "Ali"

CLOSEFILE "Students.txt"
```

---

# Closing a File

Always close the file after use.

```text
CLOSEFILE "Students.txt"
```

This saves resources and ensures data is written correctly.

---

# File Processing Flow

```
Open File

↓

Read or Write

↓

Close File
```

---

# 10.4 Abstract Data Types (ADT)

## What is an ADT?

ADT stands for **Abstract Data Type**.

An ADT combines:

- The data
- The operations that can be performed on that data

When using an ADT, we focus on **what it does**, not **how it is implemented**.

Think of a TV remote.

You press the **Volume Up** button.

You don't need to know how the electronics inside the remote work.

Similarly, when using a Stack or Queue, you only need to know which operations are available.

---

# Common ADTs

Cambridge requires students to understand:

- Stack
- Queue
- Linked List

---

# Stack

A Stack follows the rule

```
Last In

First Out

(LIFO)
```

---

## Real-Life Example

Imagine a stack of dinner plates.

```
Plate 3

Plate 2

Plate 1
```

The last plate placed on top is the first plate removed.

---

# Stack Operations

Push

Adds an item.

Pop

Removes the top item.

Peek

Looks at the top item without removing it.

---

## Example

Push A

```
A
```

Push B

```
B

A
```

Push C

```
C

B

A
```

Pop

```
Removes C
```

---

# Applications of Stack

- Undo operation
- Browser Back button
- Function calls
- Expression evaluation

---

# Queue

A Queue follows

```
First In

First Out

(FIFO)
```

---

## Real-Life Example

Students waiting outside a classroom.

```
Ali

Ahmed

Sara
```

Ali entered first.

Ali leaves first.

---

# Queue Operations

Enqueue

Add an item.

Dequeue

Remove an item.

Front

View first item.

Rear

View last item.

---

# Applications

- Printer queue
- Call centre
- Ticket booking
- CPU scheduling

---

# Linked List

A Linked List stores data in nodes.

Each node contains

```
Data

+

Link
```

The link stores the address of the next node.

---

## Example

```
+------+    +------+    +------+
| Ali  | -> | Sara | -> | John |
+------+    +------+    +------+
```

The final node points to

```
NULL
```

---

# Why Use Linked Lists?

Arrays have fixed sizes.

Linked Lists can grow or shrink whenever required.

---

# Advantages

- Dynamic size.
- Easy insertion.
- Easy deletion.
- Better memory usage.

---

# Disadvantages

- Sequential access only.
- More complex than arrays.
- Extra memory needed for links.

---

# ADTs Implemented Using Arrays

Although Stack, Queue and Linked List are different data structures, they can all be represented using arrays.

Example Stack

```
Stack[1]

Stack[2]

Stack[3]
```

The variable **Top** keeps track of the top element.

---

Queue

```
Queue[1]

Queue[2]

Queue[3]
```

Two variables are used.

```
Front

Rear
```

---

Linked List

Arrays can also store:

- Data
- Next Pointer

Example

```
Data[ ]

Next[ ]
```

Each position in the Next array stores the index of the next node.

---

# Comparison Table

| Feature | Array | Record | Stack | Queue | Linked List |
|----------|--------|---------|--------|--------|--------------|
| Stores multiple values | ✅ | ❌ | ✅ | ✅ | ✅ |
| Stores different data types | ❌ | ✅ | ❌ | ❌ | Usually No |
| Dynamic Size | ❌ | ❌ | Depends | Depends | ✅ |
| Uses Index | ✅ | ❌ | Often | Often | No |
| Easy Insertion | ❌ | N/A | Top Only | Rear Only | ✅ |

---

# Common Student Mistakes

## Data Types

❌ Using INTEGER instead of REAL.

---

## CHAR

❌ Writing

```
'AB'
```

CHAR stores only one character.

---

## Arrays

❌ Starting from index 0 when the question specifies index 1.

Always check the declaration.

---

## Records

❌ Thinking records store many students.

No.

One record stores information about **one object**.

---

## Bubble Sort

❌ Comparing random elements.

Always compare **adjacent** elements.

---

## Linear Search

❌ Stopping after checking only one element.

Search continues until the value is found or the array ends.

---

# Cambridge Examination Tips

✔ Read the array declaration carefully.

✔ Learn the difference between CHAR and STRING.

✔ Remember Record stores different data types.

✔ Remember Array stores the same data type.

✔ Bubble Sort compares adjacent values.

✔ Linear Search checks one item at a time.

✔ Stack = LIFO.

✔ Queue = FIFO.

✔ Always close files.

---

# Quick Revision Summary

## Data Types

| Type | Stores |
|------|---------|
| INTEGER | Whole numbers |
| REAL | Decimal numbers |
| CHAR | Single character |
| STRING | Text |
| BOOLEAN | TRUE/FALSE |
| DATE | Dates |

---

## Record

Stores different data types under one identifier.

---

## Array

Stores multiple values of the same data type.

---

## Bubble Sort

Compare neighbouring values and swap if necessary.

---

## Linear Search

Check every element one by one.

---

## File

Permanent storage.

---

## Stack

LIFO

Push

Pop

---

## Queue

FIFO

Enqueue

Dequeue

---

## Linked List

Nodes connected using links.

Dynamic size.

---

# Cambridge Style MCQs

### Question 1

Which data type stores decimal values?

A. INTEGER

B. BOOLEAN

C. REAL

D. CHAR

**Answer:** C

---

### Question 2

Which structure stores different data types together?

A. Array

B. Record

C. Queue

D. Stack

**Answer:** B

---

### Question 3

Which searching algorithm checks every element one by one?

A. Bubble Sort

B. Binary Search

C. Linear Search

D. Merge Sort

**Answer:** C

---

### Question 4

Which data structure follows LIFO?

A. Queue

B. Stack

C. Record

D. Array

**Answer:** B

---

### Question 5

Which operation removes an item from a queue?

A. Push

B. Peek

C. Dequeue

D. Pop

**Answer:** C

---

# Practical Exercises

1. Create an INTEGER variable called Age.

2. Create a STRING variable called StudentName.

3. Create an array to store 20 marks.

4. Write pseudocode to calculate the total marks.

5. Write pseudocode to find the maximum mark.

6. Perform Bubble Sort on

```
65

12

80

41

30
```

7. Perform Linear Search for

```
41
```

8. Create a Student Record.

9. Write pseudocode to write a student's name to a text file.

10. Explain one real-life use of:

- Stack
- Queue
- Linked List

---

# Homework

1. Explain the difference between INTEGER and REAL.

2. Explain the difference between CHAR and STRING.

3. Differentiate between Record and Array.

4. Explain Bubble Sort with an example.

5. Explain Linear Search with an example.

6. Explain why files are needed.

7. Compare Stack and Queue.

8. Explain the advantages of Linked Lists over Arrays.

---

# End of Chapter 10

Congratulations! 🎉

You have now completed **Chapter 10 – Data Types and Structures**.

After studying this chapter, you should be able to:

- Select appropriate data types.
- Create and use records.
- Create and process arrays.
- Sort data using Bubble Sort.
- Search data using Linear Search.
- Read from and write to text files.
- Explain Stack, Queue and Linked List.
- Solve Cambridge 9618 Paper 2 questions related to Data Types and Structures.

## Exam Tip

If the value contains decimal places, NEVER choose INTEGER.

Always choose REAL.
