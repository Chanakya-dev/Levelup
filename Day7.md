## ✅ Java Function Notes (Beginner Friendly)

---

### 🔹 1. `void` – No Return Value

- Used when the function **doesn’t return any data**.
- Just performs an action.

```java
public void greet() {
    System.out.println("Hello, welcome!");
}
```

✅ **Usage:**

```java
greet(); // Output: Hello, welcome!
```

---

### 🔹 2. `return` – Returns a Value

- A function can **return a value** using the `return` keyword.
- You must specify the **return type** in the method signature.

```java
public int square(int num) {
    return num * num;
}
```

✅ **Usage:**

```java
int result = square(4);  // result = 16
```

---

### 🔹 3. `static` – Called Using Class Name

- **Belongs to the class**, not an object.
- Can be called directly using the **class name** without creating an object.

```java
public static void sayHi() {
    System.out.println("Hi from static method!");
}
```

✅ **Usage:**

```java
MyClass.sayHi();  // Call directly using class name
```

---

### 🔹 4. Non-Static – Called Using Object

- Non-static methods are **associated with an object** of the class.
- You need to create an object to call them.

```java
public void sayHello() {
    System.out.println("Hello from non-static method!");
}
```

✅ **Usage:**

```java
MyClass obj = new MyClass();
obj.sayHello();
```

---

### 🔹 5. Parameters – Passing Data into Functions

- You can send input to methods using **parameters**.
- Parameters are specified inside the parentheses `()`.

```java
public void printName(String name) {
    System.out.println("Your name is: " + name);
}
```

✅ **Usage:**

```java
printName("Alice");  // Output: Your name is: Alice
```

---

## 🔚 Summary Table

| Concept      | Description                                        | How to Call                    |
|--------------|----------------------------------------------------|--------------------------------|
| `void`       | No return value                                    | `greet();`                     |
| `return`     | Returns data (int, String, etc.)                   | `int x = square(5);`           |
| `static`     | Called using class name                            | `MyClass.sayHi();`             |
| `non-static` | Called using object                                | `MyClass obj = new MyClass(); obj.sayHello();` |
| `parameters` | Pass data when calling function                    | `printName("John");`           |

---
