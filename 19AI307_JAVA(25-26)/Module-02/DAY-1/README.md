# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Car with attributes brand, model, year. Create 2 objects and print their details.

## AIM:
To create a Java class Car with attributes brand, model, and year, create two objects, and display their details.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Car class with brand, model, and year attributes.
4. Create two Car objects and assign values to their attributes.
5. Display the details of both car objects.
6. Stop the program.

## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: KESHAVARTHINI B
RegisterNumber: 212224040158
*/
```

## SOURCE CODE:

```
class Car{
    String brand;
    String model;
    int year;
}
public class prog {
    public static void main(String[] args) {
        Car car1 = new Car();
        car1.brand = "Toyota";
        car1.model = "Innova";
        car1.year = 2022;

        Car car2 = new Car();
        car2.brand = "Hyundai";
        car2.model = "i20";
        car2.year = 2021;

        System.out.println("Car 1: " + car1.brand + " " + car1.model + " " + car1.year);
        System.out.println("Car 2: " + car2.brand + " " + car2.model + " " + car2.year);
    }
}

```

## OUTPUT:
<img width="798" height="309" alt="image" src="https://github.com/user-attachments/assets/c58e337c-c13d-4284-853e-1f3d8f53bbfc" />

## RESULT:
Thus, the Java program successfully creates two Car objects and displays their details.
