# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
Create a Super class Person with fields name and age. Create a subclass Student that inherits from Person and adds a field marks (integer). Implement a method in Student called calculateGrade() which returns the grade based on the marks:

Marks ≥ 90: Grade A

Marks ≥ 75 and < 90: Grade B

Marks ≥ 50 and < 75: Grade C

Marks < 50: Grade F

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
Program to implement a Inheritance and Aggregation using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
class Person {
    String name;
    int age;

    Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
}

class Student extends Person {
    int marks;

    Student(String name, int age, int marks) {
        super(name, age);
        this.marks = marks;
    }

    String calculateGrade() {
        if (marks >= 90) {
            return "A";
        } else if (marks >= 75) {
            return "B";
        } else if (marks >= 50) {
            return "C";
        } else {
            return "F";
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String name = sc.nextLine();
        int age = sc.nextInt();
        int marks = sc.nextInt();
        Student s=new Student(name,age,marks);

        System.out.println("Name: " + s.name);
        System.out.println("Age: " + s.age);
        System.out.println("Marks: " + s.marks);
        System.out.println("Grade: " + s.calculateGrade());
    }
}
```


## OUTPUT:
<img width="502" height="592" alt="image" src="https://github.com/user-attachments/assets/548d7be1-e429-4fc4-8fb9-6fac8d6319c4" />


## RESULT:
Thus, the Java program successfully demonstrates inheritance and calculates the student's grade based on the given marks.
