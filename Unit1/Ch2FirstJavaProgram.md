Here’s a cleaner and more structured version of creating and running your first Java program:

---

### **Steps to Write and Run Your First Java Program**

#### 1. **Create a New Directory for Your Program**
```cmd
> md Abhinish
> dir
> cd Abhinish
```
This creates a folder named `Abhinish` and navigates into it.

---

#### 2. **Write Your Java Code**
1. Open **Notepad** or any text editor.  
2. Type the following code:  

```java
// Importing the default java.lang package (optional, as it's imported automatically)
import java.lang.*;

// Define the class
class MyClass {
    // The main method is the entry point of any Java program
    public static void main(String[] args) {
        // Print output to the console
        System.out.println("Hello Abhinish");
    }
}
```

3. Save the file as `MyFirst.java` in the `Abhinish` folder.

---

#### 3. **Compile Your Program**  
1. Open the **Command Prompt** and ensure you’re inside the `Abhinish` directory.  
   ```cmd
   > cd Abhinish
   ```
2. Compile the Java file using the `javac` command:  
   ```cmd
   > javac MyFirst.java
   ```
   This creates a file named `MyFirst.class`, which contains the bytecode.

---

#### 4. **Run Your Program**
1. Execute the bytecode with the `java` command:  
   ```cmd
   > java MyClass
   ```
2. Output:  
   ```
   Hello Abhinish
   ```

---

#### 5. **Verify Files**
1. To view the source code:  
   ```cmd
   > type MyFirst.java
   ```
2. To view the compiled bytecode:  
   ```cmd
   > type MyFirst.class
   ```

---

