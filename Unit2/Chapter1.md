
# Data Types : Variables and Literals

1. Data Types

Data is a important part of a program,its a ingredient of a program all the processing we do upon data. When program is running in the memory program should hold the data temporarily in the memory not permanent on the hard disk.
Where do we store the data, we store the data in the variables. Variables are ment for storing data.

In java first we declare the variable and then we can store the data.
Variables have some data type. Type of the data that we are going to store in that. We have some predefined types of data(datatypes) available in java. 

### Data Types available in java

1. Primitive data type(basic data type)giveen by the compiler of the java.

Integer :- they can have any numeric value. Without decimal point
Floating Point:- hey can have any numeric value. With decimal point
Char :- Used for storing characters.
Boolean :- For storing True and false

1 Byte = 8 Bit

Character support Unicode.

True does not mean 1 . True means true.
Default is false.

| **Category**        | **Data Type** | **Storage**   | **Range**                                         | **Default Value** |
|----------------------|---------------|---------------|--------------------------------------------------|--------------------|
| **Integral**         | **Byte**      | 1 byte        | -128 to 127                                      | `0`                |
|                      | **Short**     | 2 bytes       | -32,768 to 32,767                                | `0`                |
|                      | **Int**       | 4 bytes       | -2,147,483,648 to 2,147,483,647                  | `0`                |
|                      | **Long**      | 8 bytes       | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 | `0L`              |
| **Floating Point**   | **Float**     | 4 bytes       | ±3.4E-38 to ±3.4E+38                             | `0.0f`             |
|                      | **Double**    | 8 bytes       | ±1.7E-308 to ±1.7E+308                           | `0.0`              |
| **Character**        | **Char**      | 2 bytes       | '\u0000' (null character) to '\uFFFF'            | `'\u0000'`         |
| **Boolean**          | **Boolean**   | 1 bit (stored as 1 byte) | `true` or `false`                               | `false`            |




### How we can find the range and size of a data type ?
For every data there is a built in class available.
Primite means its a core part of compiler.

```java

import java.lang.*;

class SizeRange
{
public static void main(String arg[])
{

int x;//primitive data type
Integer y;//wraper class around int , it contains the information about int

System.out.println("Int Min:" + Integer.MIN_VALUE);
System.out.println("Int Max:" + Integer.MAX_VALUE);
System.out.println("Int Bytes " + Integer.BYTES);

}
}

```

Output:- Int Min: -2147483648
Int Max: 2147483647
Int Bytes: 4


>>> javap java.lang.Integer;
>>> javap java.lang.BYTE;
>>> javap java.lang.Short;
>>> javap java.lang.Float;
>>> javap java.lang.Character;
>>> javap java.lang.Boolean;

Every data type has their own class with their attributes.



```java

class SizeRange {
    public static void main(String arg[]) {
        byte x; // primitive data type
        Byte y; // wrapper class around byte, contains additional information about byte

        System.out.println("Byte Min: " + Byte.MIN_VALUE);
        System.out.println("Byte Max: " + Byte.MAX_VALUE);
        System.out.println("Byte Bytes: " + Byte.BYTES);
    }
}

```

Output:- Byte Min: -128
Byte Max: 127
Byte Bytes: 1

```java

class SizeRange {
    public static void main(String arg[]) {
        float x; // primitive data type
        Float y; // wrapper class around float, contains additional information about float

        System.out.println("Float Min: " + Float.MIN_VALUE);
        System.out.println("Float Max: " + Float.MAX_VALUE);
        System.out.println("Float Bytes: " + Float.BYTES);
    }
}

```

Output:- Float Min: 1.4E-45
Float Max: 3.4028235E38
Float Bytes: 4














