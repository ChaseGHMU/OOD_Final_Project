# Instance Reference

# Java
- Instance reference in Java is done by the "this" keyword. This is used to differentiate between the instance variable and the temporty variable.

Example:

```java
String name = "";

public void testMethod(name: String){
  this.string = string
}
```

# Swift
- Swift Instance variables do that same as Java instance reference, but they use "self" keyword.

```swift
PocketCaddyData.getHoles(courseId: courseId, completionHandler: { result in
  self.holes = result
  self.getPoints(self.hole)
})
```

#### Pages
[5. Classes](Classes.md)

[7. Properties](Properties.md)
