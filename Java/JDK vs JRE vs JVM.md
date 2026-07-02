
![jvm](https://media.geeksforgeeks.org/wp-content/uploads/20251003165228816476/jvm.webp "Click to enlarge")


**JDK**
-  JDK is  Java Development Kit ,it basically contains  JRE , JVM and the set of libraires
- So JDK is basically a Software package that contains the java compiler( javac ), and JRE for writing, compiling ,debugging and executing the code.
- It is platform dependent
- It also has a private virtual machine and it contains:
     - Java Runtime Environment (JRE),
     - An interpreter/loader (Java),
     - A compiler (javac),
     - An archiver (jar) and many more.
 - The  Java Runtime Environment in JDK is usually called Private Runtime because it is separated from the regular JRE and has extra content. The Private Runtime in JDK contains a JVM and all the class libraries present in the production environment, as well as additional libraries useful to developers, e.g, internationalization libraries and the IDL libraries.
 - Working of JDK
        -- ****Source Code (.java):**** Developer writes a Java program.
        - ****Compilation:**** The JDK’s compiler (javac) converts the code into bytecode stored in .class files.
        - ****Execution:**** The JVM executes the bytecode, translating it into native instructions.     

JRE

- Java Runtime Environment ,it is just for running the files and not developing them ,it includes the JVM and the libraries ,and it does not support compilation or debugging

- It is platform depenedent.
- ### Working of JRE:

1. ****Class Loading:**** Loads compiled .class files into memory.
2. ****Bytecode Verification:**** Ensures security and validity of bytecode.
3. ****Execution:**** Uses the JVM (interpreter + JIT compiler) to execute instructions and make system calls.


JVM

Java Virtual Machine is basically the engine of the Java ,responsible for converting java bytecode into the machine specific code

- Part of both JDK and JRE.
- Performs ==memory management== and ==garbage collection==.
- Provides portability by executing the same bytecode on different platforms.
 JVM implementations are platform dependent while the bytecode is platform independent and can easily run on any JVM
It heavily depends upon JIT i.e. Just in time compilation for performance

1. ****Loading:**** Class loader loads bytecode into memory.
2. ****Linking:**** Performs verification, preparation, and resolution.
3. ****Initialization:**** Executes class constructors and static initializers.
4. ****Execution:**** Interprets or compiles bytecode into native code.


### Working of JVM:

![class_loader](https://media.geeksforgeeks.org/wp-content/uploads/20251003170021775913/class_loader.webp "Click to enlarge")
## JDK vs JRE vs JVM

|Aspect|JDK|JRE|JVM|
|---|---|---|---|
|Purpose|Used to develop Java applications|Used to run Java applications|Executes Java bytecode|
|Platform Dependency|Platform-dependent (OS specific)|Platform-dependent (OS specific)|JVM is OS-specific, but bytecode is platform-independent|
|Includes|JRE + Development tools (javac, debugger, etc.)|JVM + Libraries (e.g., rt.jar)|ClassLoader, JIT Compiler, Garbage Collector|
|Use Case|Writing and compiling Java code|Running a Java application on a system|Convert bytecode into native machine code|

