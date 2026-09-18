# Ex.No:5(D) THREAD PRIORITY
## NAME: KESHAVARTHINI B
## REG NO: 212224040158
## QUESTION:
Write a java program for determine the priority and name of the current thread.

Note : Read the threadname from the User

For example:

<img width="381" height="161" alt="image" src="https://github.com/user-attachments/assets/019048d4-1291-4ab6-9864-8f3930b7c6e2" />


## AIM:
To write a Java program that reads a thread name from the user, sets the current thread’s name, and displays its priority and full thread details.

## ALGORITHM :
1. Start the program and import the necessary utilities.

2. Read a thread name from the user using a Scanner.

3. Retrieve the current thread using Thread.currentThread().

4. Set the name of the current thread using setName().

5. Obtain the thread’s priority using getPriority().

6. Display the thread’s name, priority, and full thread information.

7. End the program.





## PROGRAM:


## SOURCE CODE:
```
import java.util.Scanner;

public class CurrentThreadDetails {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String threadName = sc.nextLine();

        Thread t = Thread.currentThread();
        t.setName(threadName);

        System.out.println("Priority of Thread: " + t.getPriority());
        System.out.println("Name of Thread: " + t.getName());
        System.out.println(t);
    }
}
```


## OUTPUT:

<img width="726" height="217" alt="image" src="https://github.com/user-attachments/assets/fac09833-9da1-4690-b348-d30704a60185" />


## RESULT:

The program successfully reads a custom name for the current thread, assigns it to the running thread, and displays the thread’s priority and complete thread details.

