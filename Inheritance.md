# Inheritence/Extension

# Java
- Java uses Inheritences which allow subclasses to inherit the functions from it's superclasses. This is useful for when you want something to go in more detail than what it's parent class has. An example widely used in class is that Dog is a subclass of Pet. A Pet can be a dog and do the same thing that pets do, so they have access to the Pet methods, while also having access to any of the Dog methods. Inheritance is also used for defining that a class will use an interface.

Example:
```java
public class Dog extends Pet inherits MyInterface{

}
```

# Swift
- Swift uses extensions to allow classes to gain more methods and usability than the default class allows. You can extend any existing class to add the following things:

  - Add computed instance properties and computed type properties
  - Define instance methods and type methods
  - Provide new initializers
  - Define subscripts
  - Define and use new nested types
  - Make an existing type conform to a protocol
  
Example:

```swift
extension NewType {
  //new functionality here
}
```

#### Pages
[8. Interfaces/Protocols](InterfacesAndProtocols.md)

[10. Reflection](Reflection.md)
