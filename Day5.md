# 📘 Java Notes: **Conditionals (Decision-Making Statements)**

---

## 🧠 What are Conditionals?

Conditionals in Java are used to **make decisions** in your code. They allow your program to **execute different blocks of code depending on whether a condition is true or false**.

---

## ✅ 1. `if` Statement

### 📌 Purpose:
Executes a block **only if** the condition is true.

### 📌 Syntax:
```java
if (condition) {
    // code to execute if condition is true
}
```

### 📌 Example:
```java
int age = 20;
if (age >= 18) {
    System.out.println("You are eligible to vote.");
}
```

---

## ✅ 2. `if-else` Statement

### 📌 Purpose:
Executes one block if the condition is true, **another if it's false**.

### 📌 Syntax:
```java
if (condition) {
    // code if condition is true
} else {
    // code if condition is false
}
```

### 📌 Example:
```java
int num = 10;
if (num % 2 == 0) {
    System.out.println("Even number");
} else {
    System.out.println("Odd number");
}
```

---

## ✅ 3. `if-else if-else` Ladder

### 📌 Purpose:
Used when you have **multiple conditions** to check.

### 📌 Syntax:
```java
if (condition1) {
    // code
} else if (condition2) {
    // code
} else {
    // code if none are true
}
```

### 📌 Example:
```java
int marks = 75;
if (marks >= 90) {
    System.out.println("Grade A");
} else if (marks >= 75) {
    System.out.println("Grade B");
} else {
    System.out.println("Grade C");
}
```

---

## ✅ 4. Nested `if` Statements

### 📌 Purpose:
An `if` statement **inside another `if`** – used when decisions depend on **multiple levels** of conditions.

### 📌 Syntax:
```java
if (condition1) {
    if (condition2) {
        // code
    }
}
```

### 📌 Example:
```java
int age = 25;
boolean hasID = true;
if (age >= 18) {
    if (hasID) {
        System.out.println("Access granted");
    } else {
        System.out.println("ID required");
    }
}
```

---

## ✅ 5. `switch` Statement

### 📌 Purpose:
Used when you want to compare **one variable against many values**.

### 📌 Syntax:
```java
switch (expression) {
    case value1:
        // code
        break;
    case value2:
        // code
        break;
    default:
        // code if no match
}
```

### 📌 Example:
```java
int day = 3;
switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    case 3:
        System.out.println("Wednesday");
        break;
    default:
        System.out.println("Invalid day");
}
```

---

## 🔁 Difference: `if-else` vs `switch`

| Feature       | `if-else`                              | `switch`                         |
|---------------|----------------------------------------|----------------------------------|
| Conditions    | Can be complex (>, <, ==, &&, etc.)    | Checks only **equality**         |
| Data types    | Any type of expression                 | Limited to `int`, `char`, `enum`, `String` |
| Performance   | Slower for large checks                | Faster for multiple exact matches |
| Readability   | Less readable with many conditions     | More readable with multiple cases |

---

## 🛠 Common Use Cases

- `if`: simple checks like "is age > 18?"
- `if-else`: binary choices like "is number even or odd?"
- `if-else-if`: grading system, salary brackets
- `nested if`: login systems, role-based access
- `switch`: menu systems, day/month selectors

---
