# Reverse String

> If you want to reverse a String you can use the following method:

```java
public class Class {

    public static void main(String[] args) {
 
        String name = "Tom";
        String rname = new StringBuilder(name).reverse().toString();
 
        //Output:   name = Tom
        //          rname = moT
        
    }

}
```