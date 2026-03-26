# Constructors in Java

## What is a Constructor?

> A constructor is a special method in a class that is called when a new object of that class is created.
> The main purpose of a constructor is to set the initial states of the object's attributes and to initialize resources.
> Constructors have the same name as the class and do not have a return type, not even `void`.

## Why Do We Need Constructors?

> Constructors are important because they ensure that objects are created in a valid state.
> They allow parameters to be passed in to initialize the attributes of an object at the time of creation.
> Without constructors, developers would have to manually set all attributes after creating an object,
> which can be error-prone and impractical.

## General Syntax of a Constructor

The general syntax of a constructor looks like this:

```java
public class ClassName {
    
    // Class attributes
    private DataType attribute;

    // Constructor
    public ClassName(DataType parameter) {
        this.attribute = parameter;
    }
    
}
```
___
Example of a Constructor

Here is a simple example that shows a constructor in a class called Car:

```java

public class Car {
    
    // Class attributes
    private String brand;
    private String model;
    private int year;

    // Constructor
    public Car(String brand, String model, int year) {
        this.brand = brand;
        this.model = model;
        this.year = year;
    }
    
    // main Method
    public static void main(String[] args) {
        // Creating a new Car object
        Car myCar = new Car("Volkswagen", "Golf", 2020);
        myCar.display(); // Output: Brand: Volkswagen, Model: Golf, Year: 2020
    }

    // Method to display car information
    public void display() {
        System.out.println("Brand: " + brand + ", Model: " + model + ", Year: " + year);
    }
    
}
```
