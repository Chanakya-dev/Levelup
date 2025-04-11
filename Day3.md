# **Java Operators Notes**

## **Overview**
Operators are symbols (like `+`, `-`, `*`, `/`, `%`, etc.) that help perform operations on variables.

---

## **1. Arithmetic Operators**
These are used to perform basic mathematical operations:

- `+` : Addition  
- `-` : Subtraction  
- `*` : Multiplication  
- `/` : Division  
- `%` : Modulus (remainder)

**Example:**
```java
int a = 10;  
int b = 10;  
System.out.println(a + b);  // 20  
System.out.println(b - a);  // 0  
System.out.println(a * b);  // 100  
System.out.println(b / a);  // 1  
System.out.println(b % a);  // 0  
```

---

## **2. Assignment Operators**
These are used to assign values to variables and also perform shorthand operations:

- `=` : Assign  
- `+=` : Add and assign  
- `-=` : Subtract and assign  
- `*=` : Multiply and assign  
- `/=` : Divide and assign  
- `%=` : Modulus and assign  

**Example:**
```java
int c = a + b; // c = 20  
c /= 2;        // c = 10  
System.out.println(c);
```

---

## **3. Comparison (Relational) Operators**
Used to compare two values:

- `>`  : Greater than  
- `<`  : Less than  
- `>=` : Greater than or equal to  
- `<=` : Less than or equal to  
- `==` : Equal to  
- `!=` : Not equal to  

**Example:**
```java
System.out.println(a >= b);  // true  
System.out.println(a <= b);  // true  
System.out.println(a != b);  // false  
System.out.println(a == b);  // true  
System.out.println(a > b);   // false  
System.out.println(a < b);   // false  
```

---

## **4. Logical Operators**
Used to combine multiple conditions:

- `&&` : Logical AND (true if all conditions are true)  
- `||` : Logical OR (true if at least one condition is true)  
- `!`  : Logical NOT (inverts the result)

**Example:**
```java
System.out.println(a > b && a + b > b);      // false  
System.out.println(a > b || a + b > b);      // true  
System.out.println(!(a <= b && a + b > b));  // false  
```

---

## **5. Unary Operators**
Used to increment or decrement a value by 1:

- `++` : Increment  
- `--` : Decrement  

Can be used as:
- **Pre-increment/Pre-decrement**: `++a`, `--a`  
- **Post-increment/Post-decrement**: `a++`, `a--`

**Example:**
```java
int j = 12;  
System.out.println(--j);  // Output: 11 (Pre-decrement)
```

---
