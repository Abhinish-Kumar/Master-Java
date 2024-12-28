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



# Practical

Experiment :- 
java.lang :- contains System class , automatically important 

Experiment:- 
Why we use same name for file and class.

> javac FileName.java
> java ClassName

It will create 2 files 

1. FileName.java
2. ClassName.class

same name is good.

```java

public class ClassName{}

```
> javac File.java
>error:- class CLassName is public, should be declared in a filename ClassName.java


Solution :- two problem occurs with different name 


Experiment :- 

```java
class MyClass {
   
   public  static void main() {}}
```

> javac First.java
> java First
> Error:- Main method not found in class First. Please define main method as public static void main()
> JVM recoganize same signature


Must use same signature of main method.


Experiment :- command line argument

```java
import java.lang.*;

class MyClass{
public static void main(String arg[]){
System.out.println("Hello Abhinish");
System.out.println(arg[0]);//this one
}
}
```

>$ java javaFirstProgram.java
>Error: Could not find or load main class javaFirstProgram.java
Caused by: java.lang.ClassNotFoundException: javaFirstProgram.java

Exception error:- ArrayIndexOutOfBoundsException

Experiment :- 
>$ java javaFirstProgram.java abhinish
>Hello Abhinish
>abhinish

Whatever we type in CMD this act as a argument for our file


```java
import java.lang.*;

class MyClass{
public static void main(String arg[]){
System.out.println("Hello Abhinish");
System.out.println(arg[0]);
System.out.println(arg[1]);
}
}

```
>$ java javaFirstProgram.java abhinish kumar
>Hello Abhinish
>abhinish
>kumar

Sol:- What every argument we give along with the program name all are taken as Command line argument that is taken by program. 
You can process the data given by CMD











