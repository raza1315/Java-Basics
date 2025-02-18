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
