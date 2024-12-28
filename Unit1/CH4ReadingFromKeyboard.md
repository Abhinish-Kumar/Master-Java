## How to read the data from Keyboard

Java Provide us a class Called Scanner that we use to take the input data from the keyboard and other sources. 

eg:- keyboard
- In java we have a **unit** package or **utility package** (its a class/builin package)
- It is present in version 5 onwards
- List of methods present in Scanner class


How to use Scanner class

1. import
2. create its class


```java

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Create a Scanner object to read input
//System.in for keyboard
//System.out is associated with  monitor 
        Scanner scanner = new Scanner(System.in);
//scanner is a referance to scanner
//scanner object act as a pipe to suply input from keyboard to you

    }
}

```


```java

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
       
        Scanner scanner = new Scanner(System.in);

        int a,b,c;
        System.out.println("Enter 2 number");
        a=s.nextInt();
        b=s.nextInt();
        c=a+b;
       System.out.println("Sum is " + c); //Sum is 25
        
    }
}

```

Read two number and display sum



1. nextInt() - read integer Float
2. nextFloat()
3. nextDouble() 
4. next() - read string
5. nextLine() - read a line and sentence
6. nextByte()
7. nextShort()
8. nextLong()
9. nextBoolean()

1. hasNextInt() - return bool
2. hasNextFloat() - return bool

before reading data canform its type.



```java

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
       
        Scanner scanner = new Scanner(System.in);

       String name;
        System.out.println("May i know your name");
      name= scanner.nextLine();
       System.out.println("Welcome " + name); 
        
    }
}

```



# Practical

System.in attach to keyboard/reference of keyboard
System.out attach to monitor


```java
//must
import java.util.Scanner;

public class ReadKeyboard {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in); // Create a Scanner object for input
        System.out.print("Enter an integer: ");
        int x = sc.nextInt(); // Read an integer input
        System.out.println("You entered: " + x); // Print the input
    }
}

```


Note:- if we not import the unit package 
error> can not Find Symbol Scanner (this class is not visible or accessible to the compiler)

Note:- if give different input 
Exception> input mismatch exception


### How to find the methods of any class like Scanner

>javap java.util.Scanner
>radix will read Binary



















