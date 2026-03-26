# Scanner

##### What is a Scanner ?

> The Scanner in Java is a class from the java.util package
> used for reading input from various sources,
> such as the console, files, or strings. 
> It simplifies the process of parsing and converting input 
> into different data types (like int, double, String, etc.).

##### Why do I need it ?

- User Input: Commonly used to read input from users via the console.
- File Input: Can read data from files, making it useful for processing external data.
- Easy Parsing: Provides methods for tokenizing input, such as separating words or lines.

##### Example

```java
import java.util.Scanner; //You need to import it, for using Scanner

public class ScannerExample {
    
    public static void main(String[] args) {
        // Create a Scanner object to read input from the console
        Scanner scanner = new Scanner(System.in);

        // Prompt the user for their name
        System.out.print("Please enter your name: ");
        String name = scanner.nextLine();

        // Prompt the user for their age
        System.out.print("Please enter your age: ");
        int age = scanner.nextInt();

        // Output the entered data
        System.out.println("Hello " + name + ", you are " + age + " years old.");

        // Close the scanner
        scanner.close();
    }
}
```