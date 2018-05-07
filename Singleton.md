# Singletons
- How is a singleton implemented?
- Can it be made thread-safe?
- Can the singleton instance be lazily instantiated?

# Java
- Singletons in Java are made using the private static constructor on a class. If there isn't an object of that type already, it will return a reference of that object. An example is shown below:

```java
class Puppy {
  private static Puppy singleton = null;
  
  public String name;
  private Puppy(){
    name = "Titan";
  }
  
  public static Puppy getSingletonInstance(){
    if(singleton == null){
      singleton = new Puppy();
    }
    return singleton;
   }
}
```

To make the above code thread-safe, you would have to include the keyword "synchronized" which will invoke all other threads with that method will be suspended until it's done.

```java
class Puppy {
  private static Puppy singleton = null;
  
  public String name;
  private Puppy(){
    name = "Titan";
  }
  
  public synchronized static Puppy getSingletonInstance(){
    if(singleton == null){
      singleton = new Puppy();
    }
    return singleton;
   }
}
```

# Swift
- Swift has multiple standard ways in the Apple Framework that implements a singleton. Some of the popular ones are shown below:

```swift
let sharedURLSesson = URLSession.shared
let defaults = UserDefaults.standard
let fileManager = FileManager.default
```

Creating a singleton in swift is very easy. All you have to do is call the Singleton class to create an object that is a singleton. The init must also be overriden and made private.

```swift
final class Singleton {
  static let instance = Singleton()
  private init() {}
}
```

#### Pages
[16. Listeners and Event Handlers](ListenersAndEventHandlers.md)

[18. Programming](Programming.md)
