# Pseudocode-Docs


# 📘 Cambridge 9618 Pseudocode Notes

> Beginner Friendly | Easy English + Roman Urdu

---

# Chapter 1: Introduction to Pseudocode

## 📖 What is Pseudocode?

### Definition (Easy English)

Pseudocode is a simple way of writing the steps of a program using English words.

It is **not a programming language**, so it does not have strict syntax like Python or Java.

It is used to plan the logic of a program before writing actual code.

---

### 💬 Roman Urdu

Pseudocode ka matlab hai program ke steps ko simple English language mein likhna.

Ye **real programming language nahi hoti**.

Iska purpose sirf **program ki planning** karna hota hai.

Programmer pehle pseudocode likhta hai, phir usay Python, Java ya kisi aur programming language mein convert karta hai.

---

# 🎯 Why do we use Pseudocode?

## Advantages

- ✅ Easy to read
- ✅ Easy to understand
- ✅ Easy to write
- ✅ Easy to find mistakes
- ✅ Language independent
- ✅ Helps before writing actual code

### 💬 Roman Urdu

- Program ko samajhna easy hota hai.
- Coding se pehle planning ho jati hai.
- Mistakes jaldi mil jati hain.
- Kisi bhi programming language mein convert kiya ja sakta hai.

---

# 🔄 IPO Cycle

Har basic program isi sequence ko follow karta hai.

```text
INPUT
   ↓
PROCESS
   ↓
OUTPUT
```

### Remember

> **IPO = Input → Process → Output**

---

# 📝 Basic Program Structure

```text
DECLARE variables

INPUT values

Process

OUTPUT result
```

---

# 💻 Example 1

## Problem

Ask the user for their name and display it.

### Pseudocode

```text
OUTPUT "Enter your name"

INPUT Name

OUTPUT "Hello"

OUTPUT Name
```

### Sample Input

```text
Ali
```

### Sample Output

```text
Hello
Ali
```

---

# 🔍 Step-by-Step Explanation

## Step 1

Display a message.

```text
OUTPUT "Enter your name"
```

Screen shows:

```text
Enter your name
```

---

## Step 2

Take input from the user.

```text
INPUT Name
```

Suppose the user enters:

```text
Ali
```

Now the variable stores:

```text
Name = "Ali"
```

---

## Step 3

Display greeting.

```text
OUTPUT "Hello"
```

Output:

```text
Hello
```

---

## Step 4

Display the stored name.

```text
OUTPUT Name
```

Output:

```text
Ali
```

---

# 📚 Common Pseudocode Keywords

| Keyword | Meaning | Roman Urdu |
|----------|---------|------------|
| `DECLARE` | Create a variable | Variable banana |
| `INPUT` | Take input | User se data lena |
| `OUTPUT` | Display output | Screen par dikhana |
| `IF` | Check condition | Agar |
| `ELSE` | Otherwise | Warna |
| `ENDIF` | End IF | IF khatam |
| `FOR` | Repeat fixed times | Repeat |
| `NEXT` | End FOR | Loop khatam |
| `WHILE` | Repeat while true | Jab tak |
| `ENDWHILE` | End WHILE | WHILE khatam |
| `REPEAT` | Repeat instructions | Repeat |
| `UNTIL` | Stop when true | Jab condition true ho |
| `CASE OF` | Multiple choices | Multiple options |
| `ENDCASE` | End CASE | CASE khatam |
| `FUNCTION` | Create function | Function banana |
| `PROCEDURE` | Create procedure | Procedure banana |
| `RETURN` | Return value | Value wapas bhejna |

---

# 💻 Example 2 – Addition Program

## Problem

Input two numbers and display their sum.

### Pseudocode

```text
DECLARE Num1, Num2, Total : INTEGER

OUTPUT "Enter first number"
INPUT Num1

OUTPUT "Enter second number"
INPUT Num2

Total ← Num1 + Num2

OUTPUT Total
```

---

# ⚙️ Program Execution

### Step 1

```text
DECLARE Num1, Num2, Total : INTEGER
```

Creates three variables in memory.

---

### Step 2

```text
INPUT Num1
```

Example:

```text
10
```

---

### Step 3

```text
INPUT Num2
```

Example:

```text
20
```

---

### Step 4

```text
Total ← Num1 + Num2
```

Calculation:

```text
10 + 20 = 30
```

---

### Step 5

```text
OUTPUT Total
```

Output:

```text
30
```

---

# 🌍 Real-Life Example

Imagine a teacher calculating marks.

```text
Student tells marks
        │
        ▼
      INPUT

        │
        ▼
Teacher calculates
        │
        ▼
     PROCESS

        │
        ▼
Teacher announces result
        │
        ▼
      OUTPUT
```

Computers work in exactly the same way.

---

# 📋 Summary

- Pseudocode is **not** a programming language.
- It is used for **planning programs**.
- It is written in **simple English**.
- It is easy to read and understand.
- Most programs follow the **IPO Cycle**.

```text
INPUT
   ↓
PROCESS
   ↓
OUTPUT
```

---

# 🧠 Quick Revision

- ✅ Pseudocode is used before coding.
- ✅ It is language independent.
- ✅ It helps programmers understand logic.
- ✅ Follow the IPO cycle.

---

# ❓ Practice Questions

## Q1. What is pseudocode?

**Answer:**

Pseudocode is a simple way of writing the steps of a program using English words before writing actual code.

---

## Q2. Is pseudocode a programming language?

**Answer:**

No.

---

## Q3. Write pseudocode to input a student's name and display it.

```text
DECLARE Name : STRING

OUTPUT "Enter your name"

INPUT Name

OUTPUT "Your name is"

OUTPUT Name
```

---

## Q4. What does `INPUT` do?

**Answer:**

It takes data from the user.

---

## Q5. What does `OUTPUT` do?

**Answer:**

It displays data on the screen.

---

# 📌 Key Takeaways

- 📍 Pseudocode = Program Planning
- 📍 Uses Simple English
- 📍 Easy to Read
- 📍 Easy to Understand
- 📍 IPO = Input → Process → Output

---

## 📚 Next Chapter

**Chapter 2 – Variables & Data Types**

Topics:

- Variables
- Constants
- DECLARE
- INTEGER
- REAL
- STRING
- CHAR
- BOOLEAN
- DATE
- Arrays (Introduction)
