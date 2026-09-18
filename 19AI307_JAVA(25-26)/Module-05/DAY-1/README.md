# Ex.No:5(A) INPUTSTREAMREADER 
## NAME: KESHAVARTHINI B
## REG NO: 212224040158
## QUESTION:
Write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)
<img width="296" height="175" alt="image" src="https://github.com/user-attachments/assets/55523e5e-80b1-4fdd-9556-350840f0033c" />

## AIM:
To write a Java program that demonstrates stream chaining by connecting System.in → InputStreamReader → BufferedReader to read user input and display the entered details.

## ALGORITHM :
1. Start the program.

2. Import the necessary I/O packages (java.io.*).

3. Create a BufferedReader object by chaining System.in → InputStreamReader → BufferedReader.

4. Read the user's name using the readLine() method.

5. Read the user's age using the readLine() method.

6. Display the collected user details (name and age).

7. Handle any IOException that may occur during input operations.

## PROGRAM:


## SOURCE CODE:
```
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

public class ChainingStreamsExample {
    public static void main(String[] args) {
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));

        try {
            String name = br.readLine();
            String age = br.readLine();

            System.out.println("--- User Details ---");
            System.out.println("Name: " + name);
            System.out.println("Age: " + age);
        } catch (IOException e) {
            System.out.println("Error reading input");
        }
    }
}
```

## OUTPUT:
<img width="631" height="496" alt="image" src="https://github.com/user-attachments/assets/eab75048-8fc2-4f89-885e-bf2ccf76e182" />



## RESULT:
The program successfully demonstrates chaining of input streams using BufferedReader and InputStreamReader. It reads the user's name and age from the console and displays them without errors.
