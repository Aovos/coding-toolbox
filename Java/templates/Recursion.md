# Recursion

___

> Recursion in Java (and in programming in general) is a concept
> where a method calls itself to solve a problem (Loop, until something...)

```java
public class Recursion {

    //Data field
    int count = 0;

    //Main Method
    public static void main(String[] args) {
        Recursion2 recursion = new Recursion2();
        recursion.loop();
    }

    //Recursion Method
    public void loop() {
        if (count >= 10) {
            System.out.println(count);
            System.out.println("Program End");
        } else {
            System.out.println(count);
            count++;
            loop();
        }
    }

}
```