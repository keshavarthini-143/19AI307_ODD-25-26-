# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program that calculates the area of different shapes using method overloading. Create a class AreaCalculator with:

area(int side) for square

area(int length, int breadth) for rectangle

area(double radius) for circle


## AIM:
To demonstrate inheritance in Java by creating a Person superclass and a Student subclass that calculates a student's grade based on marks.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Person class with name and age, and extend it using the Student class with an additional marks field.
4. Initialize the inherited and student-specific fields using constructors.
5. Implement calculateGrade() using conditional statements based on the marks.
6. Create a Student object, calculate the grade, and display all details.

## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class AreaCalculator {

    int area(int side) {
        return side * side;
    }

  
    int area(int length, int breadth) {
        return length * breadth;
    }

    
    double area(double radius) {
        return Math.PI * radius * radius;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int side = sc.nextInt();
        int length = sc.nextInt();
        int breadth = sc.nextInt();
        double radius = sc.nextDouble();

        AreaCalculator obj = new AreaCalculator();

        System.out.println("Area of square: " + obj.area(side));
        System.out.println("Area of rectangle: " + obj.area(length, breadth));
        System.out.println("Area of circle: " + obj.area(radius));

       
    }
}
```


## OUTPUT:

<img width="960" height="379" alt="image" src="https://github.com/user-attachments/assets/4c5c5359-880d-41b4-a824-634caacceb64" />


## RESULT:
Thus, the Java program successfully demonstrates inheritance and calculates the student's grade based on the given marks.
