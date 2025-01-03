## What are Variables?

Variables are the names given to the data. Or variables are used for storing data. A variable must have some data type. 


```java
byte b=5;

//we are storing here 5 in b and whenever we want to get b we just have to write b.
//during the execution of the program you can change the vaule of the variable.
//Before using vaiable it must be declared first.

//declaration
byte b; //default vaule 0

//assign value to it
//Initialization of variable
byte b=5;

```

Depending on the vaule you can select datatype.

```java
int i = 175;

float f = 25.3f;

char c = "A";
```

Depending on the data type variable will ocupy memory.


```java

class IncompatibleTypesExample {
    public static void main(String[] args) {
        int x = 10.5f; // Attempting to assign a float to an int without casting
        System.out.println("Value of x: " + x);
    }
}

```

Output:- error: incompatible types: possible lossy conversion from float to int

```java

class UninitializedVariableExample {
    public static void main(String[] args) {
        int x; // Declared but not initialized
        System.out.println("Value of x: " + x); // Trying to use x without initializing
    }
}

```

error: variable x might not have been initialized



### Rules for giving variale names  (Variables - Naming Ruels)

1. Case Sensitive. (upper case Lowe case are diff)
2. Contains Alphabets,Numbers,_or$.
3. Start with Alphabets ,_ or $.
4. Should not be a keyword.
5. Should not be a class name, if class is also in use.
6. No limit on lenght of name.
7. Follow Camel Cases.


1. Case sensitive

```java

int amount;
int Amount;
//both are diff

//two variable with same name are not alloed.

```

Makes variable flexibale

2. Contains Alphabets,Numbers, _or $.

```java

int room1;
int cabin51;

int room_number;
float total$Amount;
//separaters

```

3. Starts with Alphabet,_or $.

```java

byte x1;

byte 1x; //not allowed.

```
Number can not be a starting of var

4. A variable should not be a keyword.



| **Category**                | **Keywords**                                                                 |
|-----------------------------|------------------------------------------------------------------------------|
| **Access Modifiers**         | `public`, `private`, `protected`                                            |
| **Data Types**               | `byte`, `short`, `int`, `long`, `float`, `double`, `char`, `boolean`        |
| **Class, Interface, and Enum**| `class`, `interface`, `enum`, `extends`, `implements`                      |
| **Control Flow Statements**  | `if`, `else`, `switch`, `case`, `default`, `do`, `while`, `for`, `break`, `continue` |
| **Exception Handling**       | `try`, `catch`, `finally`, `throw`, `throws`                               |
| **Modifiers**                | `abstract`, `final`, `static`, `synchronized`, `transient`, `volatile`     |
| **Object Keywords**          | `new`, `this`, `super`, `instanceof`                                       |
| **Return Control**           | `return`, `void`                                                           |
| **Packages and Imports**     | `package`, `import`                                                        |
| **Miscellaneous**            | `null`, `true`, `false`, `assert`                                          |
| **Threading**                | `synchronized`, `volatile`                                                 |
| **Others**                   | `const` (reserved), `goto` (reserved), `strictfp`, `native`                |

### Reserved Keywords:
1. **`const` and `goto`**: These are reserved but not used in Java. They cannot be used as identifiers.

Total 67

5. Should not be a class name

```java

int Interer; //not allowed

```

7. camel case (1st word of every word is capital except 1st word)




















