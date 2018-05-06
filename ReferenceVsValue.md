# References and Values
- How are the values compared? (i.e comparing two strings)

# Java
- Comparison in Java is done by both reference and value. If the two objects have the same reference, you can compare using "==". This checks if they are actually equal, while ".equals" checks things like strings to make sure they have the same value.

Example:

```java
int a = 20;
int b = 20;

if(a ==b){
  System.out.println("Equal");
}else{
  System.out.println("Not Equal");
}

String one = "Test";
String two = "Not same";

if(one.equals(two)){
  System.out.println("Equal");
}else{
  System.out.println("Not Equal");
}
```

# Swift
- Comparison in swift is pretty simple. All comparisons in swift are done with "==". This is used to compare strings, ints, or any other data type. Swift also has "===" and "!==" to compare if two objects are referencing the same object instance.

Example:

```swift
1 == 1
1 != 2

a === b
a !== b
```

#### Pages
[11. Memory Management](MemoryManagement.md)

[13. Null/Nil references](NullReferences.md)
