## Skeleton of a Java Program

### **Example Code (First.java)**

```java
// Import the language package (automatically imported)
import java.lang.*;

// Define the class
// Every Java program must have a class, and its name should match the file name.
class MyClass {
    // The main method is the entry point of any Java program.
    public static void main(String[] args) {
        // Print output to the console
        System.out.println("Hello Abhinish");
    }
}
```

---

### **Explanation**

#### **1. Class and File Name**
- Every Java program is written inside a **class**.
- The class name **must match the file name** (e.g., `MyClass` in `First.java`).

#### **2. The `main` Method**
- The **`main` method** is the starting point of any Java program.
- **Syntax**:  
  ```java
  public static void main(String[] args) { ... }
  ```

---

### **Key Points About the `main` Method**
1. **`public`**:  
   - Ensures that the method is accessible to the JVM.  
   - JVM must call the `main` method, so it must be visible.

2. **`static`**:  
   - Allows the JVM to call the `main` method without creating an object of the class.

3. **`void`**:  
   - Indicates that the method does not return any value.

4. **`String[] args`**:  
   - Used for command-line arguments. Always required.

---

### **Compilation and Execution Flow**
1. **Compile the program**:  
   ```cmd
   javac First.java
   ```
   - This generates a bytecode file named **`First.class`**.  

2. **Run the program**:  
   ```cmd
   java First
   ```
   - The JVM calls the `main` method to execute the program.

---

### **How JVM Works**
- When you run `java First`, the JVM internally calls:  
  ```cmd
  First.main()
  ```
- The JVM interprets the bytecode in `First.class` and converts it into machine code.

---





Note :- System.out.println()

Systemis a built-in class in Java.
out is a object - A static object of the `PrintStream` class.
println is its method. -  method of `PrintStream` used to print text to the console.






