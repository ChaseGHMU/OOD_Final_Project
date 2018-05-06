# Memory Management
- How is it handled?
- How does it work?
- Garbage Collection?
- Automatic Reference Counting?

# Java
- Java uses the JVM to do what they call "Mark and Sweep". There are two areas created by the JVM called the Heap and the Nursery. The heap is created when the JVM starts up and may increase or decrease in size. When the heap becomes full, garbage is collected. The nursery is the part of the heap where new objects are stored. The reasoning behind the nursery is that most objects are used temporarily and it allows for quicker collection of memory no longer being used. Java does not use Automatic Reference Counting, but instead used their Mark and Sweep design.

# Swift
- Swift utilizes Automatic Reference Counting for their memory management. Everytime you create a new instance, ARC allocates memory to store information about that current instance. It holds information about the instance itself, as well as any stored properties associated with it. When it is no longer needed, the ARC frees up the memory used by that instance so it can be used elsewhere. To make sure that ARC does not clear memory while the application is still using that instance, it keeps track of how many properties are currently referring to each class. As long as there is at least one active reference, it will not clear that information. When there are no longer any active references, it will clear the memory.

#### Pages
[10. Reflection](Reflection.md)

[12. References and Values](ReferencesVsValue.md)
