# Arrays, Loops,Imports



## Packages and import 

* To import java package into a class, we need to use java import keyword which is used to access package and its classes into the java program. Use import to access built-in and user-defined packages into your java source file so that your class can refer to a class that is in another package by directly using its name.

* Package declaration 
 
* A package is a schema object that groups logically related PL/SQL types, items, and subprograms. Use packages when writing a set of related subprograms that form an application programming interface (API) that you or others might reuse. 

* Package declaration syntax


1. Package statement (optional).
2. Imports (optional).
3. Class or interface definitions.

> package illustration;

> import java.awt.*;

> public class Drawing {
    > . . .
>}

* Imports: three options

The JOptionPane class is in the swing package, which is located in the javax package. The wildcard character (*) is used to specify that all classes with that package are available to your program. This is the most common programming style.

Example:
```
import javax.swing.*;  // Make all classes visible altho only one is used.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```
Classes can be specified explicitly on import instead of using the wildcard character.

```
import javax.swing.JOptionPane;  // Make a single class visible.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

Alternately we can the fully qualified class name without an import.
```
class ImportTest {
    public static void main(String[] args) {
        javax.swing.JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

* common import

```

import java.awt.*;	Common GUI elements.
import java.awt.event.*;	The most common GUI event listeners.
import javax.swing.*;	More common GUI elements. Note "javax".
import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
import java.io.*;	Input-output classes.
import java.text.*;	Some formatting classes.
import java.util.regex.*;	Regular expression classes.
```









## A Guide to Java Loops


*** The Java for loop is used to iterate a part of the program several times. If the number of iteration is fixed, it is recommended to use for loop.**

> There are three types of for loops in Java.

![types loop](https://static.javatpoint.com/images/java-loops.png)