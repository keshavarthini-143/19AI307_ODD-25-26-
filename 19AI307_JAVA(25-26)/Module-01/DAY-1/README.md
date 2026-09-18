# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely is applying for admission to a competitive training camp. The system checks her age and score against required criteria.

The rules are evaluated using relational operators:

Check	Operator Used  
Is her age equal to 18?	==  ,
  Is her score not equal to 100?	!=, 
   Is her score greater than 70?	>,
   Is her score less than 70?	<,
  Is her age greater than or equal to 18?	>=,
  Is her age less than or equal to 25?	<=
 
Write a program that: Takes Lovely's age and score as input, evaluates all six relational expressions and prints whether each condition is true or false.

## AIM:
To write a Java program to read Lovely's age and score and evaluate six conditions using relational operators.

## ALGORITHM :
1.	Start the program and read Lovely's age and score.
2. Evaluate the six relational expressions using ==, !=, >, <, >=, and <=.
3. Display whether each condition evaluates to true or false.
4. Stop the program.

## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: KESHAVARTHINI B
RegisterNumber: 212224040158
*/
```

## Sourcecode.java:
```
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int age =sc.nextInt();
        int score =sc.nextInt();
        System.out.println("Age == 18: " + (age ==18));
        System.out.println("Score != 100: "+ (score !=100));
        System.out.println("Score > 70: "+(score>70));
        System.out.println("Score < 70: "+(score<70));
        System.out.println("Age >= 18: "+(age>=18));
        System.out.println("Age <= 25: "+(age<=25));
    }
}
```

## OUTPUT:

<img width="875" height="509" alt="image" src="https://github.com/user-attachments/assets/42b5b5e2-ed44-4ed5-9343-ec42f7b989f1" />


## RESULT:
Thus, the Java program was successfully executed to evaluate all six relational expressions and display the corresponding true or false results.
