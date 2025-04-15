# 🔄 **LOOPS IN JAVA - Deep Explanation**

Loops are **control flow statements** that allow code to be executed repeatedly based on a condition. Instead of writing the same code again and again, loops allow us to run a block of code multiple times.

---

## ✅ 1. `for` Loop

### 📌 Purpose:
- Used when the **number of iterations is known**.
- Ideal for **count-controlled loops**.

### 📌 Syntax:
```java
for (initialization; condition; update) {
    // code block to execute
}
```

### 📌 Flow:
1. Initialization (e.g., `int i = 0`) → happens once
2. Check condition (e.g., `i < 5`)
3. If true, execute block
4. Update (e.g., `i++`)
5. Repeat from step 2

### 📌 Example:
```java
for (int i = 1; i <= 5; i++) {
    System.out.println("Count: " + i);
}
```

### 📌 Output:
```
Count: 1
Count: 2
Count: 3
Count: 4
Count: 5
```

### ✅ Use Cases:
- Printing numbers
- Iterating fixed-length lists
- Repeating steps `n` times

---

## ✅ 2. `while` Loop

### 📌 Purpose:
- Used when the **number of iterations is not known in advance**.
- Keeps running **as long as the condition is true**.

### 📌 Syntax:
```java
while (condition) {
    // code block
}
```

### 📌 Flow:
1. Check condition
2. If true, run block
3. Repeat checking condition

### 📌 Example:
```java
int i = 1;
while (i <= 5) {
    System.out.println("i = " + i);
    i++;
}
```

### 📌 Output:
```
i = 1
i = 2
i = 3
i = 4
i = 5
```

### ✅ Use Cases:
- Reading input until the user types "exit"
- Polling for updates or user action
- Loops dependent on external conditions

---

## ✅ 3. `do-while` Loop

### 📌 Purpose:
- Similar to `while`, **but always executes at least once**.
- Condition is checked **after** the loop body runs.

### 📌 Syntax:
```java
do {
    // code block
} while (condition);
```

### 📌 Flow:
1. Execute code block
2. Check condition
3. Repeat if true

### 📌 Example:
```java
int i = 1;
do {
    System.out.println("i = " + i);
    i++;
} while (i <= 5);
```

### 📌 Output:
```
i = 1
i = 2
i = 3
i = 4
i = 5
```

### ✅ Use Cases:
- Menus (show first, then ask user to repeat)
- Login attempts at least once
- Looping with guaranteed first execution

---

## ✅ 4. Enhanced `for-each` Loop *(for Arrays or Collections)*

> Though array-related, for completeness:

### 📌 Purpose:
- Designed to **simplify iteration** over collections/arrays

### 📌 Syntax:
```java
for (type variable : collection) {
    // code block
}
```

### 📌 Example:
```java
int[] nums = {10, 20, 30};
for (int n : nums) {
    System.out.println(n);
}
```

---

## 🔍 Differences Summary Table:

| Feature        | `for` Loop     | `while` Loop   | `do-while` Loop | `for-each` Loop    |
|----------------|----------------|----------------|------------------|---------------------|
| Condition First| ✅              | ✅              | ❌                | ✅                  |
| Executes At Least Once | ❌     | ❌              | ✅                | ✅ (if non-empty)    |
| Use With Arrays| ✅              | ✅              | ✅                | ✅                  |
| Index Access   | ✅              | ✅              | ✅                | ❌ (no index)       |

---

## 🧠 Best Practices:

- Use `for` when **you know how many times** the loop should run.
- Use `while` when the loop must run **until a condition is false**, and you don’t know how many iterations.
- Use `do-while` when the loop body **must run at least once**.
- Keep loops **simple and readable**; avoid infinite loops unless necessary.

---
