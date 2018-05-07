# Multithreading
- How is multitasking accomplished?
- Does the language have threads or thread-like abilites?

# Java
- Multithreading in java can be achieved by extending the Thread class. Threading is used in java to run things in a seperate background procedure so that access to the UI will not be slown in any way. An example of starting a thread is shown below:

```java
class Threading extends Thread {
  public void run(){
    try {
      System.out.println("Thread is running");
    } catch (Exception e){
      System.out.println(e);
    {
  }
}

public class MultiThread{
  public static void main(String[] args){
    int n = 10;
    for(int i = 0; i < n; i++){
      Threading obj = new Threading();
      obj.start();
    }
  }
}
```

# Swift
- Multithreading in swift is done using the DispatchQueue class. This class allows for you to create things to be handled in the background so that the UI can stay smooth and functional while running CPU intensive functions like downloading files or hitting an API to receive data. DispatchQueue has a function that does the asynchronous calls for you. An example of running a Dispatch Queue to hit an API is shown below.

```swift
let url = "Enter URL here"

URLSession.shared.datatask(with: url) { (data, response, error) in
  if error != nil {
    print(error)
  }
  
  guard let data = data else {return}
  
  do {
    let article = try? JSONDecoder().decode(from: data)
    
    DispatchQueue.main.async {
      self.article = article
    }
  }catch let error{
    print(error)
  }
}
```

#### Page
[18. Programming](Programming.md)
