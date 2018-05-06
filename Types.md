# Types

- What types does the language support?
- Are both reference and value types supported?
- Can new value types be created?

# Java

- Java has eight different primitive data types. They are int, boolean, double, float, char, byte, short, and long. Although Java directly manipulates objects by reference, it does not allow method arguments to pass by reference. Java allows you to essentially create your own data type in Classes. Classes allow you to create objects that can hold data types and methods that can be used to manipulate it. Although you can create Classes, they will still be a reference type and not a data type.

Example:

```java
boolean result = true;
int i = 10;
byte b = 8;
float f = 3.14f
```

# Swift

- Swift has two different types: Named Types and Compound Types. What other languages consider primitive types (Int, Double, Char, etc) Swift actually considers a Named Type. A compound type is a type without a name that is defined by Swift itself. These include functions and tuples. Compound types are a grop of either named types or other compound types.

Example:

```swift
//named types
var num:Int = 20
let name:String = "Chase"
let pi:Double = 3.1415

//compound types
typealias Point = (Int, Int)
let tuple: (Double, Double) = (3.1415, 9.33302)
```

#### Pages

[3. Namespaces](Namespaces.md)

[5. Classes](Classes.md)
