# 📘 Complete Notes on **Scanner Class in Java**

---

## 🔍 What is the Scanner Class?

The **`Scanner` class** is a built-in class in Java provided by the `java.util` package.  
It is used to **read input** from the **user through the keyboard** (or other input sources like files or strings).

In simple words, it allows Java programs to **accept user input at runtime**.  
This is **interactive input** like:
```bash
Enter your name: John
Enter your age: 23
```

---

## ✅ Why is Scanner Important?

- Makes your program interactive.
- Reads different types of inputs: `int`, `double`, `String`, etc.
- Easy to use.
- Widely used in competitive programming, projects, and console-based applications.

---

## 🛠️ How to Use the Scanner Class

### ✏️ Step 1: Import the Scanner Class
Before using Scanner, you must import it:
```java
import java.util.Scanner;
```

### ✏️ Step 2: Create a Scanner Object
```java
Scanner sc = new Scanner(System.in);
```
Here, `System.in` means you’re taking input from the keyboard.

---

## 🧠 Scanner Input Methods Explained

### 🔢 For Numbers:
| Method         | Input Type    | Example |
|----------------|----------------|---------|
| `nextInt()`    | Integer         | `25`    |
| `nextDouble()` | Decimal (double)| `3.14`  |
| `nextFloat()`  | Decimal (float) | `3.14f` |
| `nextLong()`   | Long number     | `1000000000` |

### 🔠 For Text:
| Method         | Reads             | Example |
|----------------|------------------|---------|
| `next()`       | Single word       | `John` |
| `nextLine()`   | Full line (with spaces) | `John Doe` |

### ✅ For Boolean:
| Method           | Input Type    |
|------------------|----------------|
| `nextBoolean()`  | `true` or `false` |

---

## 📌 Examples of Using Scanner

### 1️⃣ Reading a Number (int)
```java
import java.util.Scanner;

public class Example {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your age: ");
        int age = sc.nextInt();
        System.out.println("You are " + age + " years old.");
        sc.close();
    }
}
```

### 2️⃣ Reading a Word (next)
```java
System.out.print("Enter your city: ");
String city = sc.next();  // Expects one word only
System.out.println("City: " + city);
```

### 3️⃣ Reading a Full Line (nextLine)
```java
System.out.print("Enter your full name: ");
String name = sc.nextLine();  // Can contain spaces
System.out.println("Welcome, " + name);
```

---

## ⚠️ Common Mistake: `nextLine()` After `nextInt()`

### ❌ Problem:
```java
int age = sc.nextInt();
String name = sc.nextLine();  // Skips input
```

### 💡 Why?
- `nextInt()` leaves a newline (`\n`) in the buffer.
- `nextLine()` immediately reads it as an empty string.

### ✅ Solution:
```java
int age = sc.nextInt();
sc.nextLine(); // Clear the buffer
String name = sc.nextLine();
```

---

## 🧪 Taking Multiple Inputs in One Program

```java
Scanner sc = new Scanner(System.in);

System.out.print("Enter your name: ");
String name = sc.nextLine();

System.out.print("Enter your age: ");
int age = sc.nextInt();

System.out.print("Enter your marks: ");
double marks = sc.nextDouble();

System.out.println("Hello " + name + ", Age: " + age + ", Marks: " + marks);
sc.close();
```

---

## 🧠 Real-World Use Cases

- **Form-based input**: Name, age, gender, email
- **Menu-driven programs**: Choose options like 1. Start 2. Exit
- **Math calculators**: Take numbers and operation from user
- **Games**: Taking player names, scores
- **Condition + Scanner + Loops**: Making real apps like login validation

---

## 🧼 Closing the Scanner

Once you are done with input, always close it:
```java
sc.close();
```
This releases system resources and avoids memory leaks.

---

## 🧾 Summary

| Step                | What to Do                              |
|---------------------|------------------------------------------|
| Import Scanner      | `import java.util.Scanner;`             |
| Create Scanner      | `Scanner sc = new Scanner(System.in);`  |
| Take Input          | Use `next()`, `nextLine()`, `nextInt()` |
| Close Scanner       | `sc.close();`                            |

---

## ✅ Sample Mini Task

```java
// Ask name, age and display message
Scanner sc = new Scanner(System.in);
System.out.print("Enter your name: ");
String name = sc.nextLine();

System.out.print("Enter your age: ");
int age = sc.nextInt();

System.out.println("Hi " + name + "! You are " + age + " years old.");
sc.close();
```

---
