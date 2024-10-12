
 *The characteristics of java*

 **object**: An object in Java is **a basic unit of Object-Oriented Programming and represents real-life entities**. Objects are the instances of a class that are created to use the attributes and methods of a class. A typical Java program creates many objects, which as you know, interact by invoking methods.
 
 **interface**: A class in Java is **a set of objects which shares common characteristics/ behavior and common properties/ attributes**. It is a user-defined blueprint or prototype from which objects are created. For example, Student is a class while a particular student named Ravi is an object.
 
 **inheritance**: In Java, Inheritance means **creating new classes based on existing ones**. A class that inherits from another class can reuse the methods and fields of that class. In addition, you can add new fields and methods to your current class as well.
 
 **encapsulation**:Encapsulation in Java refers to **integrating data (variables) and code (methods) into a single unit**. In encapsulation, a class's variables are hidden from other classes and can only be accessed by the methods of the class in which they are found.
 
 **abstract**:  
Abstraction in Java refers to **hiding the implementation details of a code and exposing only the necessary information to the user**. It provides the ability to simplify complex systems by ignoring irrelevant details and reducing complexity. Java provides many in-built abstractions and few tools to create our own.

  **Polymorphism** :Polymorphism is derived from two Greek words, “poly” and “morph”, which mean “many” and “forms”, respectively. Hence, polymorphism meaning in Java refers to **the ability of objects to take on many forms**. In other words, it allows different objects to respond to the same message or method call in multiple ways.
  
*is of two types method overriding and overloading.*
**Method overriding** occurs when a subclass provides a specific implementation of a method that is already defined in its superclass. The method in the subclass should have the same name, return type, and parameters as the method in the superclass.

**Method overloading** occurs when multiple methods in the same class have the same name but different parameters (different type, number, or both).


 ```java
 //Recursion
 import java.util.*;
 public class Main{
 public static void main(String[] args)
 {
	 sayHi(2);
 }
 private static void sayHi(int count)
 {
	 if(count <=1)
	 {
	 return;
	 }
	  sayHi(--count);
 }
 }
```

```java

package JavaRecursion;

import java.util.Scanner;

public class Problem1 {

public static void main(String[] args)

{

Scanner sc =new Scanner(System.in);

int input;

input =sc.nextInt();

System.out.println(createpattern(input));

}

private static int createpattern(int input) {

for(int l=0; l<2; l++)

{

System.out.print(input);

for(int k =0 ; k<2; k++)

{

System.out.print(input-1);

for(int i=0 ; i<3 ;i++)

{

System.out.print((input-2)+"");

}

}

System.out.print(input-1);

}

return input;

}

}
```
