# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
In a haunted house, lights turn on or off based on the hour of entry:

- If the hour is even and between 2 and 6 (inclusive), lights flicker.

- If the hour is odd and between 7 and 11, lights stay off.

- If the hour is 12, lights turn red.

- Otherwise, the house is dark.

The program will print one of the following statements based on the input:

Lights flicker

Lights off

Lights red

Dark house

## AIM:
To write a Java program that uses conditional statements and logical operators to determine the light status based on the given entry hour.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the hour as input.
4. Check whether the hour satisfies the conditions for flicker, off, or red.
5. If none of the conditions match, display "Dark house".
6. Display the appropriate light status and stop the program.


## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: KESHAVARTHINI B
RegisterNumber: 212224040158
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int hour = sc.nextInt();

        if (hour % 2 == 0 && hour >= 2 && hour <= 6) {
            System.out.println("Lights flicker");
        } else if (hour % 2 != 0 && hour >= 7 && hour <= 11) {
            System.out.println("Lights off");
        } else if (hour == 12) {
            System.out.println("Lights red");
        } else {
            System.out.println("Dark house");
        }
    }
}
```

## OUTPUT:
<img width="747" height="347" alt="image" src="https://github.com/user-attachments/assets/cfe77c02-5d8f-4ee4-91b6-af7ea15ee8a3" />



## RESULT:
Thus, the Java program successfully determines and displays the light status based on the given hour.
