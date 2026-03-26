# loops

___

## What are loops?

> Loops are a fundamental programming construct that allows you
> to execute a block of code repeatedly based on a specified condition.

## Why do I need loops?

> They are essential for tasks that require repetition,
> such as iterating over arrays, processing collections,
> or performing operations until a certain condition is met.
> By using loops, you can write more efficient and concise code,
> reducing redundancy and improving maintainability.

## Which loops are there ?

| loop       | Description                                                                      |
|------------|----------------------------------------------------------------------------------|
| `for`      | Executes a block of code a specific number of times (more control & flexibility) |
| `for_each` | Iterates over elements in an array or collection                                 |
| `while`    | Executes a block of code as long as a condition is true                          |
| `do_while` | Executes a block of code at least once, then checks a condition                  |

## Loops

##### for

```java
//Syntax
for (initialization; condition; update) {
    // Code block
}
```

```java
//Example
for (int i = 0; i< 5; i++) {
    System.out.println(i);
}
```
___

##### for_each

```java
//Syntax
for (type element : array) {
    // Code block
}
```

```java
//Example
int[] numbers = {1, 2, 3, 4, 5};

for (int number : numbers) {
    System.out.println(number);
}
```

___

##### while

```java
//Syntax
while (condition) {
    // Code block
}
```

```java
//Example
int i = 0;

while (i < 5) {
    System.out.println(i);
    i++;
}
```
___

##### do_while
```java
//Syntax
do {
    // Code block
} while (condition);
```

```java
//Example
int i = 0;

do {
    System.out.println(i);
    i++;
} while (i < 5);
```