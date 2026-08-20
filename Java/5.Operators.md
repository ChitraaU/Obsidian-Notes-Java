
Java operators are symbols used to perform operations on variables and values. They play a key role in expressions, calculations, and decision-making in programs. Operators help simplify complex logic into concise statements.

- They follow a defined precedence and associativity to determine execution order.
- Some operators work on a single operand (unary), while others require two or more operands.

### ****1. Arithmetic Operators****

[Arithmetic Operators](https://www.geeksforgeeks.org/java/java-arithmetic-operators-with-examples/) are used to perform arithmetic operations on primitive numeric data types such as int, float, and double.

### ****2. Unary Operators****

[Unary Operators](https://www.geeksforgeeks.org/java/java-unary-operator-with-examples/) need only one operand. They are used to increment, decrement, or negate a value.

- Unary operators work on a single operand (`a` and `b`).
- Post-increment (`a++`) returns the value first, then increments it.
- Pre-increment (`++a`) increments first, then returns the updated value.
- Same behavior applies to decrement operators (`--`).

### ****3. Assignment Operator****

The [assignment operator](https://www.geeksforgeeks.org/java/java-assignment-operator-with-examples/) assigns a value from the right-hand side to a variable on the left. Since it has right-to-left associativity, the right-hand value must be declared or constant.
- Compound operators like +=, *=, -=, /=, %= perform operation and assignment together.
- Each statement changes the same variable, so the result depends on the previous step.

### ****4. Relational Operators****

[Relational Operators](https://www.geeksforgeeks.org/java/java-relational-operators-with-examples/) are used to check for relations like equality, greater than, and less than. They return boolean results after the comparison and are extensively used in looping statements as well as conditional if-else statements.

- Operators like >, <, >=, <=, ==, != return boolean values.
- These comparisons help in decision-making (if-else, loops).
- Each expression prints either true or false based on the condition.


### ****5. Logical Operators****

[Logical Operators](https://www.geeksforgeeks.org/java/java-logical-operators-with-examples/) are used to perform "logical AND" and "logical OR" operations, similar to AND gate and OR gate in digital electronics. They have a short-circuiting effect, meaning the second condition is not evaluated if the first is false.
- && (AND) returns true only if both conditions are true.
- || (OR) returns true if at least one condition is true.
- ! (NOT) reverses the boolean value.

### ****6. Ternary operator****

The [Ternary Operator](https://www.geeksforgeeks.org/java/java-ternary-operator/) is a shorthand version of the if-else statement. It has three operands and hence the name Ternary. 
- The ternary operator is used as a shortcut for if-else conditions.
- It evaluates multiple conditions to find the maximum among three numbers.
- Syntax: `(condition) ? value1 : value2`.
- Nested ternary operators are used here for compact decision-making.

### ****7. Bitwise Operators****

These operators perform operations at the bit level.

- [Bitwise Operators](https://www.geeksforgeeks.org/java/bitwise-operators-in-java/) manipulate individual bits using AND, OR, XOR, and NOT.
- [Shift Operators](https://www.geeksforgeeks.org/java/operators-in-java/) move bits to the left or right, effectively multiplying or dividing by powers of two.
- Operators like &, |, ^, ~ manipulate individual bits.
- Shift operators (<<, >>, >>>) move bits left or right.
- These operations are useful in low-level programming and optimizations.

### ****8. instanceof Operator****

The [instanceof operator](https://www.geeksforgeeks.org/java/instanceof-keyword-in-java/) is used for type checking. It can be used to test if an object is an instance of a class, a subclass, or an interface
- The instanceof operator checks the type of an object at runtime.
- It returns true if the object belongs to a specific class or type.
- str instanceof String confirms the type of the string object.
- It helps ensure type safety and avoid runtime errors.
