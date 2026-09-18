# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java Program to Find the Average of Array Elements.

## AIM:
To write a Java program to calculate and display the average of the elements in an array.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the number of elements and store the elements in an array.
4. Calculate the sum of all array elements using a loop.
5. Divide the sum by the number of elements to find the average.
6. Display the average up to two decimal places.

## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
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
        int n=sc.nextInt();
        int[] arr=new int[n];
        int sum=0;
        for(int i=0;i<n;i++){
            arr[i]=sc.nextInt();
            sum+=arr[i];
        }
        float avg= (float)sum/n;
        System.out.printf("The average of elements is %.2f",avg);
    }
}
```

## OUTPUT:

<img width="901" height="498" alt="image" src="https://github.com/user-attachments/assets/13a33984-8426-48c2-98e0-52d564fd27f2" />


## RESULT:
Thus, the Java program successfully calculates and displays the average of the given array elements.
