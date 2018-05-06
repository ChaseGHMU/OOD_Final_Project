# Properties
- Getters and Setters.. write your own or built in?
- Backing variables?
- Computed properties?

# Java
- Properties in Java contain key and value pairs and are a subclass of hashtables. They are used to get properties from private classes that you need information from. It can also be used to get properties from the system.

Example:

```java
import java.util.*
import java.io.*

[...]

Properites p = new Properties();
System.out.println(p.getproperty("name"));
```

# Swift
- Swift allows you the ability to write your own getters and setters. They are optional and allow yoou to set other properties and values inderectly. They can be used to define computed properties and set other properties.

Example from Swift's documentation:

```swift
struct Rect {
    var origin = Point()
    var size = Size()
    var center: Point {
        get {
            let centerX = origin.x + (size.width / 2)
            let centerY = origin.y + (size.height / 2)
            return Point(x: centerX, y: centerY)
        }
        set(newCenter) {
            origin.x = newCenter.x - (size.width / 2)
            origin.y = newCenter.y - (size.height / 2)
        }
    }
}
```

#### Pages

[6. Instance Reference](InstanceReference.md)

[8. Interfaces/Protocols](InterfacesAndProtocols.md)
