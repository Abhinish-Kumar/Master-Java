


## Literals in Java  

Literals are constant values directly written into the code that represent fixed data. They are used to initialize variables or for computations in the program.  

### Types of Literals in Java  

1. **Integer Literals**  
   - Represents whole numbers without decimal points.  
   - Example:  
     ```java
     int x = 10;  // 10 is an integer literal
     int y = 0x1A; // Hexadecimal literal (26 in decimal)
     ```

2. **Double Literals**  
   - Represents numbers with decimal points.  
   - Example:  
     ```java
     double pi = 3.14159;  // A double literal
     ```

3. **Character Literals**  
   - Represents a single character enclosed in single quotes.  
   - Example:  
     ```java
     char grade = 'A';  // 'A' is a character literal
     ```

4. **String Literals**  
   - Represents a sequence of characters enclosed in double quotes.  
   - Example:  
     ```java
     String name = "John";  // "John" is a string literal
     ```

5. **Long Literals**  
   - Represents long integer values by appending `L` or `l` to the number.  
   - Example:  
     ```java
     long distance = 10000000000L;  // 'L' indicates this is a long literal
     ```

6. **Float Literals**  
   - Represents floating-point numbers by appending `F` or `f` to the number.  
   - Example:  
     ```java
     float temperature = 98.6F;  // 'F' indicates this is a float literal
     ```

7. **Boolean Literals**  
   - Represents logical values: `true` or `false`.  
   - Example:  
     ```java
     boolean isJavaFun = true;  // true is a boolean literal
     ```

8. **Double Literals with Explicit Declaration**  
   - Double literals can also have `D` or `d` appended, though it’s optional.  
   - Example:  
     ```java
     double value = 42.0D;  // 'D' indicates this is a double literal
     ```

---

### Example Program:  
```java
public class LiteralsExample {
    public static void main(String[] args) {
        int age = 25;              // Integer literal
        double height = 5.9;       // Double literal
        char initial = 'A';        // Character literal
        String name = "Alice";     // String literal
        long population = 7800000000L;  // Long literal
        float weight = 65.5F;      // Float literal
        boolean isCodingFun = true; // Boolean literal
        
        System.out.println("Age: " + age);
        System.out.println("Height: " + height);
        System.out.println("Initial: " + initial);
        System.out.println("Name: " + name);
        System.out.println("Population: " + population);
        System.out.println("Weight: " + weight);
        System.out.println("Is coding fun? " + isCodingFun);
    }
}
```


## Integer literals can be represented in various number system.

1. Decimal number system -- 0 to 9 (10 digits)
2. Binary -- 0,1 (2 digit)
3. Octal -- 0 to 7 (8 digit)
4. Hexadecimal -- 0 to 9 + A to F (16 digit)



```java

public class NumberSystemsExample {
    public static void main(String[] args) {
        int decimal = 123;         // Decimal literal
        int binary = 0b1010;       // Binary literal
        int octal = 012;           // Octal literal
        int hexadecimal = 0xA;     // Hexadecimal literal

        System.out.println("Decimal: " + decimal);
        System.out.println("Binary: " + binary);
        System.out.println("Octal: " + octal);
        System.out.println("Hexadecimal: " + hexadecimal);
    }
}
```

```html
Decimal: 123  
Binary: 10  
Octal: 10  
Hexadecimal: 10  

```


Note :- you can use _ with numbers 


If you have bigger Figure you can separate the digits with _.

```java
class Literal
{
public static void main(String arg[]){
long l=999_999_999;
float f=12_456.56f;
System.out.println(f);
System.out.println(l);
}
}
```












