# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To write a Java program to reverse a given string.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the string from the user.
4. Initialize an empty string to store the reversed string.
5. Traverse the string from the last character to the first and append each character.
6. Display the reversed string.

## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
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
        String str=sc.nextLine();
        String rev="";
        for(int i=str.length()-1;i>=0;i--){
            rev=rev+str.charAt(i);
        }
        System.out.println("Reversed string: "+rev);
    }
}
```


## OUTPUT:

<img width="831" height="291" alt="image" src="https://github.com/user-attachments/assets/6051a41c-0a9d-49ab-98c3-945907244319" />


## RESULT:
Thus, the Java program successfully reverses and displays the given string.
