# Nil/Null References
- Which does the language use?
- Does the language have features for handling null/nil references?

# Java
- Java uses null to specify when there is nothing there. There is no fancy way of checking if something is null or not, just if statements that you must use to check if the value is null or not.

Example:

```java
String test = null;

if(test == null){
  System.out.println("There's nothing here!");
}
```

# Swift
- Swift uses nil references instead of null. Swift handles nil references by having data types have the ability to be optional, which means they can no be initiated which would give them the value of nil. You will then use an if let statement that will check to see if there is anything there, and if so it will allow the code inside the block to be ran.

Example:

```swift
var test:String?

if let test = test{
  print("This line of code will not be ran")
}

test = "Hello World"

if let test = test {
  print("This line will since test now has a value!")
}
```

#### Pages

[12. References and Values](ReferenceVsValue.md)

[15. Lambda Expressions and Closures](LambdasAndClosures.md)
