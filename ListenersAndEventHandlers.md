# Listeners and Event Handlers

# Java
- In Java, events are handled by listener interfaces. These are used to wait for a something to happen, such as a button being clicked or the size of the page changing in size. You must implement the interface that you want to use to make the listener happen.

Example:

```java
stage.heightProperty().addListener((ObservableValue<? extends Number> observable, Number oldValue, Number newValue) -> {
  boardHeight = newValue.doubleValue();
  create();
});
```

# Swift
- Swift apps handle event using responder object. These objects are an instance of UIResponder. When an event is received, the UIKit automaticall directs that event to its appropriate responder.

#### Pages

[15. Lambda Expressions and Closures](LambdasAndClosures.md)

[17. Singleton](Singleton.md)
