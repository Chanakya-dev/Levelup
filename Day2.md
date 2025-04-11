# **Java Data Types Notes**

## **Overview**
Data types specify the type of data that a variable can hold. Java is a statically typed language, so variables must be declared with a data type.

## **Definition**
Data-type is a keyword which helps you to know which type of data you are Storing in a Variable
---

## **1. Primitive Data Types**
Java has 8 primitive data types categorized as follows:

### **Numeric Types:**

- **byte** – 1 byte – Stores whole numbers from -128 to 127  
- **short** – 2 bytes – Stores whole numbers from -32,768 to 32,767  
- **int** – 4 bytes – Stores whole numbers from -2³¹ to 2³¹-1  
- **long** – 8 bytes – Stores whole numbers from -2⁶³ to 2⁶³-1 (add `L` at the end)

### **Floating-Point Types:**

- **float** – 4 bytes – Stores fractional numbers (add `f` at the end)  
- **double** – 8 bytes – Stores larger fractional numbers (default for decimals)

### **Character Type:**

- **char** – 2 bytes – Stores a single character (e.g., 'A')

### **Boolean Type:**

- **boolean** – 1 bit – Stores `true` or `false` only

---

## **2. Non-Primitive (Reference) Data Types**
- Includes classes, arrays, interfaces, and strings.
- Example: `String`, `Array`, `Object`, etc.
- Can be used to call methods, unlike primitives.

---

## **Example Usage:**
```java
int age = 25;
float height = 5.9f;
char grade = 'A';
boolean isPassed = true;
String name = "John";
```

---

## **Default Values of Primitive Data Types:**
| Data Type | Default Value |
|-----------|----------------|
| byte      | 0              |
| short     | 0              |
| int       | 0              |
| long      | 0L             |
| float     | 0.0f           |
| double    | 0.0d           |
| char      | '\u0000'       |
| boolean   | false          |

---
