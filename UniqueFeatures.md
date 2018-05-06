# Unique Features

- Does the language have any particularly unique features?

# Java

- Java doesn't have too many unique features due to the fact that most languages today have been built as being an answer or a response to Java. Java does have the JVM though which in itself is pretty unique as it allows you to compile to code that will be interpreted by the JVM itself so that it has an ease of use that can be run on any machine anywhere.

# Swift
- Swift's main unique feature is that it has a great solution to the nil/null error which comes in the form of failables. These allow you to have values that have the potential to be nil. It also comes with the ability to "unwrap" the failable variable to be used only if is in not nil. An example of how failables look is below.

```swift
var myName: Int?
    
//uses if let statement to check if variable is 
//able to unrwrap before printing it.
if let myName = myName {
  print(myName)
}
```

#### Pages
[1. Language Purpose](LanguagePurposes.md)

[3. Namespaces](Namespaces.md)
