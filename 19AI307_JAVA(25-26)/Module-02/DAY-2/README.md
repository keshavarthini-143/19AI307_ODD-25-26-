# Ex.No:2(B) METHODS

## QUESTION:
Write a method int square(int number) that returns the square of a given number.

## AIM:
To write a Java method square(int number) that calculates and returns the square of a given number.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a method square() that accepts an integer number.
4. Calculate the square by multiplying number by itself.
5. Return the calculated value.
6. Display the returned square value.


## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
public class Main{
    int square(int num){
        return num*num;
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        Main o=new Main();
        System.out.println(o.square(n));
    }
}
```


## OUTPUT:

<img width="468" height="226" alt="image" src="https://github.com/user-attachments/assets/15cd2458-d78f-43e3-8cd1-e8e6a94b0b4d" />


## RESULT:
Thus, the Java method successfully calculates and returns the square of the given number.
