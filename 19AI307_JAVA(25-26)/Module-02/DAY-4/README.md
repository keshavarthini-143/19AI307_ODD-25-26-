# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a Java program to demonstrate a parameterized constructor.

## AIM:
To write a Java program to demonstrate the use of a parameterized constructor by initializing and displaying employee details.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create an Employee class with name and id attributes.
4. Define a parameterized constructor to initialize the employee details.
5. Read the employee name and ID, then create an object using the constructor.
6. Display the employee name and ID.

## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
class Employee{
    String name;
    int id;
    Employee(String name, int id){
        this.name=name;
        this.id=id;
        
    }
    void disp(){
        System.out.println("Employee Name: "+name);
        System.out.println("Employee ID: "+id);
    }
}
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        
        String name=sc.nextLine();
        int id=sc.nextInt();
        Employee emp=new Employee(name,id);
        emp.disp();
    }
    
}
```


## OUTPUT:
<img width="663" height="336" alt="image" src="https://github.com/user-attachments/assets/ccde0392-ee42-48a7-8620-62d8c2c54902" />



## RESULT:
Thus, the Java program successfully demonstrates a parameterized constructor and displays the initialized employee details.
