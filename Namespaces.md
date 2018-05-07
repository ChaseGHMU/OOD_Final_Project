# Namespaces

- How are name spaces implemented?
- How are name spaces used?

# Java
- Namespaces in Java are handled by packages. Each package proveds protection to namespaces. So, two packages could have files with the same name in it, but the package is used to differentiate between the files. To create a package you must include that package keyword at the beginning of the file.

Example:
```java

package TestPackage;
public interface MyInterface{
  //interface functionality here
}

package TestPackage;
public class FancyClass implements MyInterface {
  //class functionality here
}

```

# Swift
- Namespacing in swift is implicit and they are all scoped by the module they are in. There is no need for prefixes. Namespaces are also not per file, but instead by target.

Example:

```swift
import UIKit
import PackageB

PackageB.test()
```

#### Pages

[2. Unique Features](UniqueFeatures.md)

[4. Types](Types.md)
