# SwitchCase

##### What is SwitchCase ?

> The switch statement in Java is a control structure 
> that allows you to execute different code blocks based on the value
> of a variable -> alternative to long `if-else` chains

##### Why do I need SwitchCase ?

- Readability
- Efficiency
- Grouping Cases
- Enum Handling
- Default Handling

##### Example

```java
public class Switch_Case_ {

    public static void main(String[] args) {
        int month = 11; // example November
        switch (month) {
            case 1:
            case 01: // multiple cases for the same code block -> reducing redundancy   
                System.out.println("January");
                break;
            case 2:
                System.out.println("February");
                break;
            case 3:
                System.out.println("March");
                break;
            case 4:
                System.out.println("April");
                break;
            case 5:
                System.out.println("May");
                break;
            case 6:
                System.out.println("June");
                break;
            case 7:
                System.out.println("July");
                break;
            case 8:
                System.out.println("August");
                break;
            case 9:
                System.out.println("September");
                break;
            case 10:
                System.out.println("October");
                break;
            case 11:
                System.out.println("November");
                break;
            case 12:
                System.out.println("December");
                break;
            default:
                System.out.println("no month");
        }
    }
}
```