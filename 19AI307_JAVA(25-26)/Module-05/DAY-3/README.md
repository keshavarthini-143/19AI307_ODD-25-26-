# Ex.No:5(C)  FILE HANDLING USING JAVA
## NAME: KESHAVARTHINI B
## REG NO: 212224040158
## QUESTION:
Write a Java program to create a new file named example.txt.

 <img width="290" height="147" alt="image" src="https://github.com/user-attachments/assets/a6a67b4f-be79-4940-8ee1-e0c734a79fa5" />

## AIM:
To write a Java program that demonstrates basic file handling by creating a new file using the File class and the createNewFile() method.

## ALGORITHM :
1. Start the program and import the required java.io.File package.

2. Create a File object and specify the filename to be created.

3. Call the createNewFile() method to attempt file creation.

4. Check if the file is successfully created.

5. If created, display the file name to the user.

6. Handle any exceptions that may occur during file creation.

7. End the program.	





## PROGRAM:

## SOURCE CODE:

```
import java.io.File;

public class CreateFileExample {
    public static void main(String[] args) {
        try {
            File file = new File("example.txt");
            if (file.createNewFile()) {
                System.out.println("File created: " + file.getName());
            }
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```
## OUTPUT:
<img width="740" height="195" alt="image" src="https://github.com/user-attachments/assets/43e4a17c-1424-4fa2-84b0-c186a1eb5a7e" />



## RESULT:
The program successfully creates a new file named example.txt in the project directory. If the file already exists, the program simply terminates without creating a duplicate.

