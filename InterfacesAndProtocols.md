# Interfaces/Protocols
- What does the language support?
- What abilities does it have?
- How is it used?

# Java
- Java supports the uses of interfaces. Interfaces are used to define a list of methods that a class has to implement if it inherits from that class. Interfaces can also only contain method signatures and fields. It is used to help acheive polymorphism and ensure that every calss that implements from that interface has those methods needed.

Example:

```java
public interface MyInterface {
  public void helloWorld();
  public void interfaceFunction();
}
```

# Swift
- Swift uses protocols instead of interfaces. Protocols in swift are essentially blueprints for a class to implement. The protocol is a list of requirements that your class, struct, or enum must conform to. It is used as a way to help "build" your function to use.

Example:

```swift
protocol SomeProtocol {
  //definition goes here
}
```

#### Pages

[7. Properties](Properties.md)

[9. Inheritance/Extension](Inheritance.md)
