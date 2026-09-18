# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 
## NAME: KESHAVARTHINI B
## REG NO: 212224040158
## QUESTION:
Write a Java program to serialize a collection of objects (like ArrayList<Student>) into a file.
<img width="690" height="260" alt="image" src="https://github.com/user-attachments/assets/009cda3f-7124-4cfe-af33-bb8be9b4e19a" />

## AIM:
To write a Java program that demonstrates object serialization and deserialization, where multiple Student objects entered by the user are stored in a file and later retrieved and displayed.

## ALGORITHM :
1. Start the program and import required I/O and utility packages.

2. Create a Student class that implements Serializable.

3. Read the number of students and their details from the user and store them in a list.

4. Open an ObjectOutputStream and write the list of Student objects to a file.

5. Open an ObjectInputStream and read back the list of Student objects from the file.

6. Display the deserialized student details on the screen.

7. Handle all I/O exceptions that occur during serialization and deserialization.

## PROGRAM:

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

// Student class must implement Serializable
class Student implements Serializable {
    private static final long serialVersionUID = 1L;

    private int id;
    private String name;
    private double marks;

    public Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    @Override
    public String toString() {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class StudentSerializationUserInput {

    // Serialize list of students
    public static void serializeStudents(List<Student> students, String fileName) {
        try (ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream(fileName))) {
            oos.writeObject(students);
            System.out.println("Students serialized successfully into: " + fileName);
        } catch (IOException e) {
            System.out.println("Error during serialization: " + e.getMessage());
        }
    }

    // Deserialize list of students
    @SuppressWarnings("unchecked")
    public static List<Student> deserializeStudents(String fileName) {
        List<Student> students = null;
        try (ObjectInputStream ois = new ObjectInputStream(new FileInputStream(fileName))) {
            students = (List<Student>) ois.readObject();
            System.out.println("Students deserialized successfully from: " + fileName);
        } catch (IOException | ClassNotFoundException e) {
            System.out.println("Error during deserialization: " + e.getMessage());
        }
        return students;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        List<Student> students = new ArrayList<>();

        int n = scanner.nextInt();
        scanner.nextLine(); // consume newline

        // Read student details
        for (int i = 0; i < n; i++) {
            int id = scanner.nextInt();
            scanner.nextLine();
            String name = scanner.nextLine();
            double marks = scanner.nextDouble();
            scanner.nextLine();
            students.add(new Student(id, name, marks));
        }

        String fileName = "students.dat";

        // Serialize
        serializeStudents(students, fileName);

        // Deserialize
        List<Student> deserializedStudents = deserializeStudents(fileName);

        // Display deserialized data
        if (deserializedStudents != null) {
            System.out.println("\nDeserialized Students:");
            for (Student s : deserializedStudents) {
                System.out.println(s);
            }
        }

        scanner.close();
    }
}
```





## OUTPUT:

<img width="1242" height="449" alt="image" src="https://github.com/user-attachments/assets/3b1213d3-934c-4356-9b52-f1f29494a618" />


## RESULT:
The program successfully serializes a list of Student objects into a file named students.dat and then deserializes the data back into a list. It correctly displays all the retrieved student information, proving that object serialization and deserialization work as expected.
