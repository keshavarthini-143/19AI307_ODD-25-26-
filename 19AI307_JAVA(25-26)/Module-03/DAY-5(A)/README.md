# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program to demonstrate an inner class by creating a class Inner inside an Outer class and accessing a variable of the outer class.

## AIM:
To write a Java program to demonstrate the use of an inner class and access the members of the outer class

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create an Outer class with an integer variable and define an Inner class inside it.
4. Create a display() method in the inner class to access the outer class variable.
5. Create objects of the Outer and Inner classes.
6. Call the display() method and print the value.


## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: KESHAVARTHINI B
RegisterNumber: 212224040158
*/
```

## SOURCE CODE:

```
class Outer {
    int number = 10;

    class Inner {
        void display() {
            System.out.println("Number: " + number);
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Outer outer = new Outer();
        Outer.Inner inner = outer.new Inner();

        inner.display();
    }
}
```

## OUTPUT:
<img width="387" height="129" alt="image" src="https://github.com/user-attachments/assets/a06af543-b5ce-4b77-b17a-3dbe6948ce28" />



## RESULT:
Thus, the Java program successfully demonstrates the creation and use of an inner class in Java.
