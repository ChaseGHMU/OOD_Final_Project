# Errors and Exception Handling

# Java
- Exceptions are handled in Java by using try catch statements. Anything that has a chance to fail or anything that can be stopped while happening, like file reading and writing, needs to be done in try catch statements. The try block is where the code is written and the catch is used to handle any exceptions that come up while happening. An example of try catch blocks is shown below.

```java
 File file = fileChooser.showOpenDialog(stage);
        if (file != null) {
            
            BufferedReader bufferedReader = null;
            String document = "";
                    
            try {
                bufferedReader= new BufferedReader(new FileReader(file));
                
                String line = "";
                
                while ( (line = bufferedReader.readLine()) != null) {
                    document += line;
                }
                
            } catch (FileNotFoundException fnfex) {
                throw fnfex;
            } catch (IOException ioex) {
                throw ioex;
            } finally {
                if (bufferedReader != null) {
                    try {
                        bufferedReader.close();
                    } catch (Exception ex) {
                        throw ex;
                    }
                }
            }
            try{
                parseFile(document);
            }catch(Exception ex){
                Alert alert = new Alert(AlertType.INFORMATION);
                alert.setHeaderText("Empty File");
                alert.setContentText("The JSON you are trying to load is either empty or not suitable for this program."
                                    + "Please try a different file.");
                alert.showAndWait();
                throw ex;
            }
        }
```

# Swift
- Swift has optionals and optional chaining to help with a lot of error handling, but sometimes it is useful to have an explanation on why the function has failed. That's why swift give you the ability to throw erros if something goes wrong. Errors are represented typically by an enum with diffent casses of errors that can be thrown. This extends the Error protocol.

```swift
enum HomeworkError: Error {
  case notLongEnough
  case insufficentAnswers
  case blankChoices
}
```

The enum above is used to represent potential errors that can come up when handling homework. To throw one of the errors it is as simple as:

```
throw HomeworkError.notLongEnough(needed: 500)
```

#### Pages
[12. References and Values](ReferenceAndValue.md)

[14. Null/Nill references](NullReferences.md)
