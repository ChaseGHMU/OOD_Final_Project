# Lambdas and Closures

# Java
- Lambdas in Java are essentially a simpler way of doing Anonymous Inner Classes. Ideally, they are used when the inner class will have few methods so that it can be more compactly and efficiently read since Inner classes can get confusing and excessive.

Example:

```java
stage.heightProperty().addListener((ObservableValue<? extends Number> observable, Number oldValue, Number newValue) -> {
  boardHeight = newValue.doubleValue();
  create();
});
```

# Swift
- Closures are self-contained blocks of functionality that can be passed around and used. They are nested functions in the sense that that have self-defined blocks of code that are run at a seperate time. An example from The Swift documentation uses an example of creating a function to reverse sort a string. The example is shown below.

An array of strings like the one below:
```swift
let name = ["Chase", "Scott", "Aaron", "Tyler"]
```

Has a function called "sorted(by:) that takes in a function. This can be used to create a closure that is used only that time for doing the sort needed. For instance:

```swift
reversed = name.sorted(by: { (string1: String, string2: String) -> Bool in 
  return s1 > s2
})
```

This closure will reverse the array by string order. The array will then look like:

```swift
print(name) //["Tyler", "Scott", "Chase", "Aaron"]
```

#### Pages

[12. References And Values](ReferenceVsValue.md)

[15. Listeners and Event Handlers](ListenersAndEventHandlers)
