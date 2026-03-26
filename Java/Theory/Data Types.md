# Data Types

___

##### Introduction

> In Java, primitive data types are the most basic data types that represent single values.
> They are not objects and are predefined by the language. 
> Primitive data types can be categorized into several groups based on their characteristics: 
> integer types, floating-point types, character types, and boolean types. 
> Below is a table that organizes these data types by their groups and sorts them by size within each group.
> 
> This organization provides a clear overview of the primitive data types in Java, their sizes, and their respective descriptions and examples.
 

##### Integer Types

| Data Type  | Size (in Bits) | Description                                                                         | Example            |
|------------|----------------|-------------------------------------------------------------------------------------|--------------------|
| byte       | 8              | Integer value ranging from -128 to 127	                                             | byte b = 100;      |
| short      | 16             | Integer value ranging from -32,768 to 32,767                                        | short s = 1000;    |
| int        | 32             | Integer value ranging from -2,147,483,648 to 2,147,483,647                          | int number = 10;   |
| long       | 64             | Integer value ranging from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807  | long l = 100000L;  |


##### Floating-Point Types
| Data Type  | Size (in Bits)  | Description                            | Example           |
|------------|-----------------|----------------------------------------|-------------------|
| float      | 32              | Single-precision floating-point number | float f = 5.75f;  |
| double     | 64              | Double-precision floating-point number | double pi = 3.14; |

##### Character Type
| Data Type  | Size (in Bits)  | Description              | Example            |
|------------|-----------------|--------------------------|--------------------|
| char       | 16              | Single Unicode character | char letter = 'A'; |

##### Boolean Type
| Data Type  | Size (in Bits)       | Description                           | Example                |
|------------|----------------------|---------------------------------------|------------------------|
| boolean    | 1 (not standardized) | Represents a truth value (true/false) | boolean isTrue = true; |