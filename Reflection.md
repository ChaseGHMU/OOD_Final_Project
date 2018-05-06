# Reflection
- What reflection abilities are supported?
- How is reflection used?

# Java
- Java allows reflection to get information like the class, method, and constructors. This information is used to figure out how classes work on the inside so you have a better idea of what to expect from it's constructors and methods.

Example:

```java
Test obj = new Test();
Class class = obj.getClass();
System.out.prinln("Class Name: " + class.getName());
```

# Swift
- Swift does not allow reflection at the moment.

#### Pages
[9. Inheritance/Extensions](InheritanceAndExtensions.md)

[11. Memory Management](MemoryManagement.md)
