# Javadoc

___

## Javadoc class

```java
/**
 * The <ClassName> class represents <a brief description of the class>.
 *
 * @author <authorname>
 * @version <version number / date>
 *
 */
class Javadoc {

    //...

}
```

___

## Javadoc method

```java
//...

    /**
     * Adds two numbers together.
     * This method takes two double values as parameters and returns their sum.
     * It can be used for basic arithmetic operations in a calculator application.
     * 
     * @param num1 the first number to be added
     * @param num2 the second number to be added
     * @return the sum of num1 and num2
     */
    public double add(double num1, double num2) {
        return num1 + num2;
    }
    
//...
```

___

## Javadoc Tags

| Tag                         | Description                                                                   |
|-----------------------------|-------------------------------------------------------------------------------|
| `@param`                    | Describes a method's parameters                                               |
| `@return`                   | Describes the return value of a method                                        |
| `@throws` (or `@exception`) | Describes an exception that may be thrown by the method                       |
| `@author`                   | Specifies the name of the author of the class or method                       |
| `@version`                  | Specifies the version number of the class or method                           |
|                             |                                                                               |
| `@todo`                     | Indicates a task that needs to be completed                                   |
| `@since`                    | Indicates the version in which the class or method was introduced             |
| `@see`                      | Refers to related classes, methods, or documentation                          |
| `@link`                     | Inserts a link to another class or method in the Javadoc documentation        |
| `@deprecated`               | Marks a method or class as deprecated and suggests an alternative             |
|                             |                                                                               |
| `@inheritDoc`               | Inherits documentation from the superclass or interface                       |
| `@code`                     | Marks a code snippet that should be displayed in the Javadoc                  |
| `@value`                    | Used to document the value of a static field                                  |
| `@default`                  | Specifies the default value for a parameter (typically used with annotations) |
|                             |                                                                               |
| `@apiNote`                  | Provides additional information about the API                                 |
| `@implSpec`                 | Describes the implementation specification of a method or class               |
| `@implNote`                 | Provides additional implementation notes                                      |