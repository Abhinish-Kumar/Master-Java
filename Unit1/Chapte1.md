# Download and install JDK


JDK (Java Development Kit) Inside it we have JRE and JVM.

JDK is used for developing java programs. 
It has development tools that are useful for compiling java program or debugging tools are available.

And once you write the code you need to execute and for executing it we need JRE (Java Runtime environment) 

JDK=Development tools + JRE 
JRE = Java Class Library + JVM

JVM actualy executes our java program. 


Here is a diagram in code markdown format that represents the architecture of JDK, JRE, and JVM. 

```plaintext
+--------------------------------------+
|               JDK                    |
|  +-------------------------------+   |
|  |            JRE                |   |
|  |  +-------------------------+  |   |
|  |  |         JVM             |  |   |
|  |  |  +-------------------+  |  |   |
|  |  |  |   Class Loader    |  |  |   |
|  |  |  +-------------------+  |  |   |
|  |  |  | Bytecode Verifier |  |  |   |
|  |  |  +-------------------+  |  |   |
|  |  |  |   Interpreter      |  |  |   |
|  |  |  +-------------------+  |  |   |
|  |  |  | JIT Compiler      |  |  |   |
|  |  |  +-------------------+  |  |   |
|  |  +-------------------------+  |   |
|  |                               |   |
|  |   Java Class Library          |   |
|  +-------------------------------+   |
|                                      |
|     Development Tools (Compiler,    |
|     Debugger, etc.)                 |
+--------------------------------------+
```

### Explanation:

1. **JDK (Java Development Kit)**:
   - The outermost layer containing:
     - **Development Tools**: Compiler, debugger, etc.
     - **JRE (Java Runtime Environment)**: Necessary for running Java programs.

2. **JRE (Java Runtime Environment)**:
   - Contains:
     - **Java Class Library**: Pre-built classes and methods for use in Java applications.
     - **JVM (Java Virtual Machine)**: Core component for executing Java programs.

3. **JVM (Java Virtual Machine)**:
   - Consists of:
     - **Class Loader**: Loads class files.
     - **Bytecode Verifier**: Ensures code correctness and security.
     - **Interpreter**: Converts bytecode to machine instructions.
     - **JIT Compiler**: Optimizes code for better performance during execution.




## How flow 

1. We create file Firt.java----> Javac-----> First.class -----> Java First

First javac compiler which is a part of JDK convert it to first.class and then first .class is converetd by java compiler which is  a part of JRE and Internally it uses JVM 


Compilation is done by Javac compiler which is a part of JDK
and execution is done by java which is a part of JRE 

javac is a development tool 
and java is a run time environment 



Here's a visual markdown diagram that explains the flow of Java compilation and execution:

```plaintext
+-----------------------+       +----------------------+       +----------------------+
|      First.java       |       |      First.class     |       |     Java Program     |
|  (Source Code File)   |       |  (Bytecode File)     |       |  (Execution Output)  |
+-----------------------+       +----------------------+       +----------------------+
            |                            |                              |
            |  javac (JDK: Compiler)     |                              |
            +--------------------------->|                              |
                                         |  java (JRE: Executor)        |
                                         +----------------------------->|

```


Flow Explanation:
1. **First.java**:
   - The source code written in Java.

2. **Javac (Java Compiler)**:
   - A part of **JDK** (Java Development Kit).
   - Converts the source code into **First.class**, which is bytecode (intermediate representation).

3. **First.class**:
   - A platform-independent bytecode file.

4. **Java (JRE)**:
   - A runtime environment responsible for executing Java programs.
   - Takes the bytecode file and runs it.

5. **JVM (Java Virtual Machine)**:
   - Internally used by **java** (JRE).
   - Executes the bytecode by interpreting or compiling it into machine code.

### Key Points:
- **JDK**: Contains tools for development (e.g., `javac` compiler).
- **JRE**: Provides the environment to run the program (e.g., `java` command).
- **JVM**: Handles bytecode execution within the JRE.



## Installation of JDK

https://www.oracle.com/java/technologies/downloads/#java23

x64 Installer - download 

program files > java 

java -version check this in CMD


If not working set the path 

Steps to set the path in windows

program files > java > jdk-17 > bin 

copy this path

OnThis PC -> right click > property > advance system settings >environment variable >path (above is for the user and below for teh entire system) > edit >new >paste your path > ok 


Here's a simplified step-by-step guide to installing JDK and setting the path on Windows:  

---

### **1. Download JDK**  
1. Visit the [Oracle JDK Downloads page](https://www.oracle.com/java/technologies/downloads/#java23).  
2. Look for the **x64 Installer** and download it.  

---

### **2. Install JDK**  
1. Open the downloaded file and follow the installation wizard.  
2. During installation, JDK will be installed in a default location:  
   **`C:\Program Files\Java\jdk-<version>`**.  

---

### **3. Check Installation**  
1. Open the **Command Prompt (CMD)** by searching for "cmd" in the Start menu.  
2. Type the following command and press **Enter**:  
   ```cmd
   java -version
   ```  
3. If the installation was successful, you’ll see the installed Java version.  

---

### **4. If Java is Not Recognized**  
If you get an error saying "Java is not recognized," you need to set the **Path** environment variable.  

---

### **5. Find the JDK Bin Path**  
1. Go to the folder where JDK was installed:  
   **`C:\Program Files\Java\jdk-<version>`**.  
2. Open the `bin` folder. For example:  
   **`C:\Program Files\Java\jdk-17\bin`**.  
3. Copy the full path from the address bar.  

---

### **6. Set the Path Variable**  
1. Right-click on **This PC** (or My Computer) and select **Properties**.  
2. On the left side, click **Advanced System Settings**.  
3. In the **System Properties** window, click the **Environment Variables** button.  

---

### **7. Edit the Path Variable**  
1. Under **User Variables** (for your user account) or **System Variables** (for all users), look for the **Path** variable.  
2. Select **Path** and click **Edit**.  
3. In the Edit Environment Variable window:  
   - Click **New**.  
   - Paste the copied JDK `bin` path (e.g., `C:\Program Files\Java\jdk-17\bin`).  
   - Click **OK**.  

---

### **8. Verify the Path**  
1. Open the Command Prompt again and type:  
   ```cmd
   java -version
   ```  
2. You should now see the installed Java version displayed.

---

### **Why Set the Path?**  
- Setting the Path allows the system to find Java commands (`java`, `javac`, etc.) from any directory.  
- Without it, you’d need to navigate to the JDK `bin` folder every time to use Java commands.

---









