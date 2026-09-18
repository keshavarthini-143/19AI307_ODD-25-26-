# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class. Take input from the user.

## AIM:
To write a Java program to check whether a given number is an Armstrong number using Math.pow() and the Integer wrapper class.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read the number as input and use the Integer wrapper class to obtain its value.
4. Count the number of digits and extract each digit from the number.
5. Use Math.pow() to calculate the sum of each digit raised to the number of digits.
6. Compare the sum with the original number and display whether it is an Armstrong number.



## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
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

        String input = sc.nextLine();
        Integer num = Integer.valueOf(input);

        int original = num;
        int digits = input.length();
        int sum = 0;
        int temp = num;

        while (temp != 0) {
            int digit = temp % 10;
            sum += (int) Math.pow(digit, digits);
            temp /= 10;
        }

        if (sum == original)
            System.out.println(original + " is an Armstrong number.");
        else
            System.out.println(original + " is not an Armstrong number.");

        
    }
}
```
## OUTPUT:
<img width="867" height="252" alt="image" src="https://github.com/user-attachments/assets/d6ccd49d-ff14-4ce8-b35d-0ba4fb3fbde3" />


## RESULT:
Thus, the Java program successfully checks whether the given number is an Armstrong number using Math.pow() and the Integer wrapper class.
