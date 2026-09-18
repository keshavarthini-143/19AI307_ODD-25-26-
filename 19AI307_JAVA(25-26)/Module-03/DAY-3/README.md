# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create abstract class BankAccount with method calculateInterest(). Extend it in SavingsAccount and FixedDepositAccount.

## AIM:
To demonstrate abstraction and runtime polymorphism by creating an abstract BankAccount class and implementing calculateInterest() in SavingsAccount and FixedDepositAccount.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create an abstract BankAccount class with the abstract method calculateInterest().
4. Extend it with SavingsAccount and FixedDepositAccount, implementing the interest calculation for each.
5. Read the user's choice and corresponding account details, then create the appropriate object.
6. Call calculateInterest() and display the interest rounded to 2 decimal places.

## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: KESHAVARTHINI B
RegisterNumber: 212224040158
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

abstract class BankAccount {
    abstract double calculateInterest();
}

class SavingsAccount extends BankAccount {
    double balance;

    SavingsAccount(double balance) {
        this.balance = balance;
    }

    double calculateInterest() {
        return balance * 0.04; 
    }
}

class FixedDepositAccount extends BankAccount {
    double amount;
    int years;

    FixedDepositAccount(double amount, int years) {
        this.amount = amount;
        this.years = years;
    }

    double calculateInterest() {
        return amount * 0.07 * years; 
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int choice = sc.nextInt();
        BankAccount account;

        if (choice == 1) {
            double balance = sc.nextDouble();
            account = new SavingsAccount(balance);
        } else {
            double amount = sc.nextDouble();
            int years = sc.nextInt();
            account = new FixedDepositAccount(amount, years);
        }

        System.out.printf("%.2f", account.calculateInterest());
    }
}

```

## OUTPUT:
<img width="431" height="363" alt="image" src="https://github.com/user-attachments/assets/b2f15571-8a43-43f6-907f-f84cb3eabd5d" />

## RESULT:
Thus, the Java program successfully demonstrates abstraction and runtime polymorphism by calculating interest for different types of bank accounts.
