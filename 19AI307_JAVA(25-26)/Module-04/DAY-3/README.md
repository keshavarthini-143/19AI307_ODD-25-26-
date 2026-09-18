# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:
Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).

## AIM:
To develop a Java program that models a Library containing multiple Book objects, where books are created and managed within the Library.
## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a Library object.
4. Read the number of books.
5. Repeat for each book:
6. Read the book title.
7. Read the author name.
8. Create the Book object inside the Library.
9. Add the book to the collection.
10. Display the details of all books in the Library.
11. Stop the program

## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: KESHAVARTHINI B
RegisterNumber:  212224040158
*/
```

## SOURCE CODE:
```
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }
        library.showBooks();
        sc.close();
    }
}
class Book {
    private String title;
    private String author;
    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }
    public String getDetails() {
        return title + " by " + author;
    }
}
class Library {
     ArrayList<Book> books = new ArrayList<>();
    public void addBook(String title, String author) {
        Book b = new Book(title, author);
        books.add(b);
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        for (Book b : books) {
            System.out.println("- " + b.getDetails());
        }    
    }
}

```

## OUTPUT:
<img width="885" height="518" alt="image" src="https://github.com/user-attachments/assets/7084df60-6a07-4528-84b0-ddb5c14fab74" />



## RESULT:
The program was executed successfully. The Library managed multiple Book objects, and the details of all books were displayed correctly.
