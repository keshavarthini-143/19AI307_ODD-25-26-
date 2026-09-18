# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:
Write a program that reads two integers and divides the first by the second. Handle the case when division by zero occurs.

## AIM:
To write a Java program that reads two integers and divides the first integer by the second, while handling division-by-zero errors using exception handling.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Scanner object to read input.
4. Read two integers, a and b.
5. Use a try block to divide a by b.
6. If division is successful, display the result.
7. If b is zero, catch the ArithmeticException.
8. Display an error message: "Error: Division by zero".
9. Stop the program.





## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: KESHAVARTHINI B
RegisterNumber: 212224040158
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int a= sc.nextInt();
        int b=sc.nextInt();
        try{
            int c=a/b;
            System.out.println("Result: "+c);
        }catch(ArithmeticException e){
            System.out.println("Error: Division by zero");
        }
    }
}
```

## OUTPUT:

<img width="696" height="312" alt="image" src="https://github.com/user-attachments/assets/439b54be-52d9-4c59-a0ab-61ed8eeb498c" />


## RESULT:
The program was executed successfully. It correctly performs division when the second number is non-zero and handles the division-by-zero exception by displaying an appropriate error message.
