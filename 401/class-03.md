# Maps, primitives, File I/O

## Primitives vs. Objects

1. 
```
// primitive type
int x = 5;

// Object type
Integer = 5
```
2. Objects need more space in memory:
**Sizes :**

*For Primitives*:

* boolean – *1 bit*
* byte – *8 bits*
* short, char – *16 bits*
* int, float – *32 bits*
* long, double – *64 bits*

*For Objects*:

* Boolean – *128 bits*
* Byte – *128 bits*
* Short, Character – *128 bits*
* Integer, Float – *128 bits*
* Long, Double – *192 bits*

3. Primatives' live in the Stack while Objects live in Heap.
4. We use wrapper classes for objects .
5. Objects require more time to perform operations.
6. Default values for wrapper classes are null.
7. Objects and wrapper classes to use collections.


## Scanner Objects

1. Breaking Input into Tokens.
2. Treats all input tokens as simple String values.
3. Supports tokens for all of the Java language's primitive types (except for char), as well as BigInteger and BigDecimal.
4. We have to mention the locale, because thousands separators and decimal symbols are locale specific.

## Exceptions 

**In Java “an event that occurs during the execution of a program that disrupts the normal flow of instructions” is called an exception. This is generally an unexpected or unwanted event which can occur either at compile-time or run-time in application code.**

### Types of Exception in Java with Examples
1. ArithmeticException. It is thrown when an exceptional condition has occurred in an arithmetic operation.
2. ArrayIndexOutOfBoundsException.
3. ClassNotFoundException.
4. FileNotFoundException. 
5. IOException. 
6. InterruptedException. 
7. NoSuchFieldException. 
8. NoSuchMethodException.

![call stack](https://static.javatpoint.com/core/images/types-of-exception-in-java.png)

![searching for exception](https://www.w3spoint.com/wp-content/uploads/2014/08/Pasted-into-Exception-handling-in-java-1.png)

1. Checked ex. `java.io.FileNotFoundException` /*Subject*
2. Runtime ex. `java.io.IOError` / can not read file because of system or hardware /*Not Subject*
3. Error ; programming bugs, such as logic errors or improper use of an API , ex. `NullPointerException` /*Not Subject*

Exception Handler components -->*try, catch & finally*