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



## Installation 














