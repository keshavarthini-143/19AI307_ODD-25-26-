# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class College with a final variable universityName = "Saveetha University". Create objects and print the name.
## AIM:
 To create a class College with a final variable universityName = "Saveetha University". Create objects and print the name.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a College class with a final variable universityName.
4. Assign "Saveetha University" to the final variable.
5. Create an object of the College class.
6. Access and display the value of the final variable.
## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:

```
import java.util.*
class College {
    final String universityName = "Saveetha University";
}

class prog {
    public static void main(String[] args) {
       College c=new College();
       System.out.println(c.universityName);
    }
}
```

## OUTPUT:
<img width="630" height="185" alt="image" src="https://github.com/user-attachments/assets/c7ed5ac4-6543-4150-bd5f-9983425e7772" />


## RESULT:
Thus, the Java program successfully demonstrates the use of the final keyword to create a constant variable.
