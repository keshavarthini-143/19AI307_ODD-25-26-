# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
In mathematics, the factorial of a non-negative integer n, denoted as n!, is the product of all positive integers less than or equal to n. For example:

5! = 5 × 4 × 3 × 2 × 1 = 120

3! = 3 × 2 × 1 = 6

0! is defined as 1.

Write a Java program that prompts the user to enter a non-negative integer and then calculates and displays the factorial of the given number.

- Use a for loop to perform the calculation.

- Make sure to handle the case when the user enters 0.

- Display the result in a clear and user-friendly way.

## AIM:
To write a Java program to calculate and display the factorial of a non-negative integer using a for loop.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read a non-negative integer n from the user and initialize factorial = 1.
4. Use a for loop from 1 to n to calculate the factorial.
5. Display the factorial; for 0, the result remains 1.
6. Stop the program.


## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int num = sc.nextInt();
        long fact=1;
        for(int i=1;i<=num;i++){
            fact=fact*i;
        }
        System.out.println("Factorial of " + num +" is: " + fact);
    }
}
```

## OUTPUT:
<img width="810" height="309" alt="image" src="https://github.com/user-attachments/assets/3790540e-e0cb-4d95-a000-7eb55933d998" />


## RESULT:
Thus, the Java program successfully calculates and displays the factorial of the given non-negative integer.
