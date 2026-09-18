# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:

Write a Java program to create a class called Circle with a private instance variable radius. Provide public getter and setter methods to access and modify the radius variable. However, provide two methods called calculateArea() and calculatePerimeter() that return the calculated area and perimeter based on the current radius value. 


## AIM:
To create a Java Circle class with a private radius variable and public getter, setter, area, and perimeter methods.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Circle class with a private radius and public getter and setter methods.
4. Define methods to calculate the area and perimeter using the current radius.
5. Read the radius, set it using the setter, and calculate the area and perimeter.
6. Display the radius, area, and perimeter.

## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Circle {
   
    private double radius;

  
    public double getRadius() {
        return radius;
    }

   
    public void setRadius(double radius) {
        this.radius = radius;
    }

    
    public double calculateArea() {
        return Math.PI * radius * radius;
    }

   
    public double calculatePerimeter() {
        return 2 * Math.PI * radius;
    }
}

public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        Circle cir=new Circle();
        double radius = sc.nextDouble();
        cir.setRadius(radius);
        System.out.printf("Radius: %.2f\n" ,cir.getRadius());
        System.out.printf("Area: %.2f\n", cir.calculateArea());
        System.out.printf("Perimeter: %.2f\n", cir.calculatePerimeter());
        
    }    
}
```


## OUTPUT:
<img width="644" height="304" alt="image" src="https://github.com/user-attachments/assets/2fc36f94-edec-4b4d-a0f7-b7e42911a923" />

## RESULT:
Thus, the Java program successfully calculates and displays the area and perimeter of the circle using the given radius.
