
**Main Method**
Syntax of the main() method is always written as:

![2056957879](https://media.geeksforgeeks.org/wp-content/uploads/20260429090033516230/2056957879.webp "Click to enlarge")

The main method is the starting point of the program the JVM executes the code starting from here only
The java.exe method launcher initalizes the JVM using JNI and then it invokes the main method

Here the public is the access modifier while static is the keyword which means that object creation is not requires void is the return type while main is the specific name of the function which the JVM kooks for and the String args is the array of string type which accepts the Java command line arguments

And the point to note here is that the main method can be overloaded.


**Constant and Variable**

Variable is basically the storage location in the computer's  memory that holds a value while constant is the fixed value that is generally stored in a variable.

**Comment and Documentation**

In any programming language when we code it considered a good practice to write comments or make documentation for the code as it generally helps other developers to understand your code better.

**Variable naming convention**

While name a variable we use pascal case convention and it should not use special characters , numbers at the start and in Java the name of the variable is case sensitive.

**DATA TYPES**
Basically there are two broad division of the data types:
 - **Primitive or Built in data types** which include
 integer,
 float
 double
 char
 boolean
 byte
 short
 long
and all of these stores the values directly into the memory

|Type|Description|Default|Size|Example|Range|
|---|---|---|---|---|---|
|boolean|Logical values|false|Not JVM-defined|true, false|true or false|
|byte|8-bit signed integer|0|1 byte|10|-128 to 127|
|char|16-bit Unicode character|\u0000|2 bytes|'A', '\u0041'|0 to 65,535|
|short|16-bit signed integer|0|2 bytes|2000|-32,768 to 32,767|
|int|32-bit signed integer|0|4 bytes|1000, -500|-2,147,483,648 to 2,147,483,647|
|long|64-bit signed integer|0L|8 bytes|123456789L|±9.22e18|
|float|32-bit floating point|0.0f|4 bytes|3.14f|~6–7 digits precision|
|double|64-bit floating point|0.0d|8 bytes|3.14159d|~15–16 digits precision|
AND 
- **Non -primitive /Derived data types**
String
Array
Class
object
interface and all of these stores memory addresses or memory references rather than the actual value.
 