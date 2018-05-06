# Classes
 - Defining Classes
 - Creating new instances
 - Constructing/Initializing
 - Destructing/de-initializing
 
# Java

### Defining
- Defining classes in Java involves defining whether the class will be public, private, or protected followed by the name of the class. A class can have both static and dynamic methods and can also have both static and dynamic methods. Static methods can only access static variables though due to the fact that dynamic class methods are not available until the creation of the class, while static methods are created at compile time.

Example:

```java
public class NewClass {
  //define class here
}
```

### Creating new instances
- creating an instance of a class happens in a different class or object. This is used by the "new" keyword which lets the compiler know to create a new instance of that class. After creating the new instance, it allows you access to the instance variables and methods. The instance can be created with nothing as default, or can take parameters passed in to help construct the instance.

Example:

```java
//no parameters
Puppy dog = new Puppy();

//with parameters
Puppy dog = new Puppy("Titan", 2);
```

### Constructing
- Constructors are used to define an instance at creation. By default, Java instances are initialized with no constructor parameters. You can create as many constructors as you want for your class, or you can create none.

Example:

```java
public Puppy(){
  //blank constructor
}

public Puppy(String name, Int age){
  self.name = name;
  self.age = age;
}
```

### Destructing
- Java as a language has a garbage collector to handle when to destruct instances, so destructing typically isn't done by the creator themselves. The garbage collector waits until an object no longer has references to it or when it hasn't been used in awhile.

# Swift

### Defining
- Defining a class in Swift is as simple as typing "class" followed by what you want the class name to be. Swift allows you to use both Classes and Structs in you code. The keyword for creating a struct is "struct"

Example:

```swift
class NewClass{
  //implement Class logic here
}

struct NewStuct {
    //implement Struct logic here
}
```

### Creating new instances
- Creating new instances in Swift is similar to in Java except that swift doesn't require the "new" keyword. Creating an instance is as simple as naming whatever class you want to create followed by the parameters needed to create that class.

Example:

```swift
//no parameters
let puppy = Puppy()

//with parameters
let puppy = Puppy(name: "Titan", age: 2)
```

### Constructing
- Swift constructors are called Initializers and uses the "init" keyword. Initializers are used for the same purpose as they are in Java, which is allowing parameters to be passed in to help define the instance being created.

Example:

```swift
class Puppy{
  var name: String
  var age: Int
  
  init(){
    name = "No Name"
    age = 1
  }
  
  init(name: String, age: Int){
    self.name = name
    self.age = age
  }
}
```

### Destructing
- Swift, like Java, handles deallocating your instances for you when they are no longer needed. It handles memory management through Automatic Reference Counting (ARC). You do not typically net to deallocate yourself, but if needed there is the "deinit" keyword to handle deallocation of the instance.

Example:

```swift
class Puppy {
  deinit {
    //handle deallocation of instance
  }
}
```

#### Pages

[4. Types](Types.md)

[6. Instance Reference](InstanceReference.md)
