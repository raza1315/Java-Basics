# **📌 What is Java?**  
Java is a **high-level, object-oriented, platform-independent** programming language used for:  
✅ Web applications  
✅ Mobile apps (Android)  
✅ Backend development (Spring Boot)  
✅ Game development  
✅ Desktop apps  

### **Why Java?**
- **Platform Independent** 🎯 → Write once, run anywhere!  
- **Object-Oriented** 📦 → Helps structure large programs.  
- **Secure & Fast** 🔒⚡ → Used in enterprise applications.  
- **Huge Community Support** 👨‍💻👩‍💻 → Many learning resources available.

---

# **📌 Java Installation (Mac)**
### 1️⃣ **Install Java (JDK)**
Java Development Kit (**JDK**) includes:
- **javac** → Compiler (turns `.java` files into `.class` files)
- **java** → JVM (Java Virtual Machine) runs the `.class` files  

### **Install via Homebrew (Recommended)**
```sh
brew install openjdk
```
For a specific version (e.g., Java 17):
```sh
brew install openjdk@17
```
Then, set the **JAVA_HOME** path:
```sh
echo 'export PATH="/opt/homebrew/opt/openjdk/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```
Check installation:
```sh
java -version
```

### 2️⃣ **Install VS Code & Java Extension**
- Download VS Code from [here](https://code.visualstudio.com/)
- Install **"Extension Pack for Java"** in VS Code.

---

# **📌 Java Code Execution Flow**
### **1️⃣ Writing Java Code**  
Create a file **`Main.java`**:
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```

### **2️⃣ Compile the Code**
Run in the terminal:
```sh
javac Main.java
```
🔹 This generates `Main.class` (bytecode file).

### **3️⃣ Run the Compiled Code**
```sh
java Main
```
🔹 The **JVM** (Java Virtual Machine) executes `Main.class` and prints:
```
Hello, Java!
```

---

# **📌 Understanding Java Execution Flow**
### 🚀 **How Java Works Internally**
1. **Write Code (`.java` file)** → You write Java code.
2. **Compilation (`javac`)** → Java compiler converts the code into **bytecode (`.class` file)**.
3. **Execution (`java`)** → JVM reads the bytecode and runs it on any OS.

🔹 Unlike Python, Java **must** be compiled before running.  
🔹 Java doesn’t run code **directly** but instead uses **JVM** for execution.

---

# **📌 Key Java Concepts for Beginners**
### **1️⃣ Variables & Data Types**
```java
int age = 25;
double price = 10.5;
char grade = 'A';
String name = "John";
boolean isJavaFun = true;
```

### **2️⃣ Control Statements**
#### **If-Else Statement**
```java
int age = 18;
if (age >= 18) {
    System.out.println("You are an adult.");
} else {
    System.out.println("You are underage.");
}
```

#### **Loops**
🔹 **For Loop**
```java
for (int i = 1; i <= 5; i++) {
    System.out.println("Count: " + i);
}
```
🔹 **While Loop**
```java
int i = 1;
while (i <= 5) {
    System.out.println("Number: " + i);
    i++;
}
```

### **3️⃣ Functions (Methods)**
```java
public class Main {
    public static void greet() {
        System.out.println("Hello, Java!");
    }

    public static void main(String[] args) {
        greet();  // Calling the function
    }
}
```

### **4️⃣ Object-Oriented Programming (OOP) Basics**
#### **Classes & Objects**
```java
class Car {
    String brand;
    int speed;

    void drive() {
        System.out.println(brand + " is driving at " + speed + " km/h.");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();
        myCar.brand = "Tesla";
        myCar.speed = 100;
        myCar.drive();
    }
}
```
✔ `Car` is a **class** (blueprint).  
✔ `myCar` is an **object** (instance of class).  
✔ Methods like `drive()` define behavior.


---
---
# ***Next Section***

---
---

# **📌 Java Basics for Beginners**  
## **1️⃣ Variables & Data Types**
In Java, variables must have a **specific type**:  

```java
public class Main {
    public static void main(String[] args) {
        int age = 25;            // Integer
        double price = 99.99;    // Decimal number
        char grade = 'A';        // Single character
        String name = "Raza";    // Text
        boolean isJavaFun = true; // True/False

        System.out.println("Age: " + age);
        System.out.println("Price: " + price);
        System.out.println("Grade: " + grade);
        System.out.println("Name: " + name);
        System.out.println("Is Java fun? " + isJavaFun);
    }
}
```
🔹 **Java is strongly typed** → You must define a type for each variable.

---

## **2️⃣ Control Statements**
### **✔ If-Else**
```java
int num = 10;
if (num > 0) {
    System.out.println("Positive Number");
} else {
    System.out.println("Negative Number");
}
```

### **✔ Switch Statement**
```java
int day = 2;
switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    default:
        System.out.println("Other day");
}
```

---

## **3️⃣ Loops**
Loops help **repeat code** multiple times.

### **✔ For Loop**
```java
for (int i = 1; i <= 5; i++) {
    System.out.println("Count: " + i);
}
```

### **✔ While Loop**
```java
int i = 1;
while (i <= 5) {
    System.out.println("While Loop: " + i);
    i++;
}
```

### **✔ Do-While Loop (Runs At Least Once)**
```java
int i = 1;
do {
    System.out.println("Do-While Loop: " + i);
    i++;
} while (i <= 5);
```

---

## **4️⃣ Arrays in Java**
Arrays store **multiple values** in one variable.

### **✔ Single-Dimensional Array**
```java
public class Main {
    public static void main(String[] args) {
        int[] numbers = {10, 20, 30, 40, 50};

        System.out.println("First element: " + numbers[0]); // Output: 10

        // Loop through an array
        for (int i = 0; i < numbers.length; i++) {
            System.out.println("Element at index " + i + ": " + numbers[i]);
        }
    }
}
```
🔹 `numbers.length` gives the array size.  
🔹 Indexing starts from **0**.

### **✔ Multi-Dimensional Array**
```java
public class Main {
    public static void main(String[] args) {
        int[][] matrix = {
            {1, 2, 3},
            {4, 5, 6},
            {7, 8, 9}
        };

        System.out.println("Element at [1][2]: " + matrix[1][2]); // Output: 6

        // Printing the 2D array
        for (int i = 0; i < 3; i++) {
            for (int j = 0; j < 3; j++) {
                System.out.print(matrix[i][j] + " ");
            }
            System.out.println();
        }
    }
}
```
🔹 Used for tables, matrices, grids.  
🔹 **`matrix[i][j]`** accesses elements.

---

## **5️⃣ Methods (Functions)**
Methods help reuse code.

### **✔ Defining and Calling Methods**
```java
public class Main {
    // Method without parameters
    static void sayHello() {
        System.out.println("Hello, Java!");
    }

    // Method with parameters
    static void greet(String name) {
        System.out.println("Hello, " + name + "!");
    }

    public static void main(String[] args) {
        sayHello();
        greet("Raza");
    }
}
```
🔹 **Methods make code reusable.**  
🔹 **Static methods** belong to the class and don’t need an object to be called.

### **✔ Method with Return Type**
```java
public class Main {
    static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int sum = add(10, 5);
        System.out.println("Sum: " + sum);
    }
}
```
🔹 **Returns a value instead of printing it.**

---

## **6️⃣ Object-Oriented Programming (OOP) Basics**
Java is **object-oriented**, meaning it works with **classes** and **objects**.

### **✔ Creating a Class and Object**
```java
class Car {
    String brand;
    int speed;

    void drive() {
        System.out.println(brand + " is driving at " + speed + " km/h.");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car(); // Object created
        myCar.brand = "Tesla";
        myCar.speed = 100;

        myCar.drive();
    }
}
```
🔹 **`Car` is a class** (a blueprint).  
🔹 **`myCar` is an object** (an instance of the class).  

### **✔ Constructor (Special Method to Initialize Objects)**
```java
class Person {
    String name;

    // Constructor
    Person(String newName) {
        name = newName;
    }

    void sayName() {
        System.out.println("My name is " + name);
    }
}

public class Main {
    public static void main(String[] args) {
        Person p1 = new Person("Raza");
        p1.sayName(); // Output: My name is Raza
    }
}
```
🔹 A **constructor** runs **automatically** when an object is created.  
🔹 It **initializes values** when an object is made.


---
---
---
