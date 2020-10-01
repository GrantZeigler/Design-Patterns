# Grant Zeigler - Design patterns


## Design Pattern 1: Bridge

### Problem:
This is used in situations when the abstractiona and the implementation need to be developed separately. Can also be used when the program only needes to access one and not the other.

### Solution: 
The solution is to create a "bridge" between the implementation and the abstraction. Doing this will allow for loose coupling between the abstraction and the implementation.


### Consequences: 
* Decoupling interface and implementation - Allows for the implementation to be changed or switched at runtime. Also allows for
* Improved extensibility - gain the ability to extend the implementationa and the abstraction indepentently, allowing for more specialized code 
* Hiding implementation details from clients - Clients won't be able to access data that they should not be able to acess


## Design Pattern 2: Decorator AKA Wrapper

### Problem:
Used when you want to add responsibilities to specific objects and not the whole class.

### Solution:
Create an object that encapsulates the specific component that you want to add things to.

### Consequences: 
* More flexible than normal inheritance
* Avoids very complex classes high in the hierarchy
* A decorator and its component aren't identical
* Lots of little objects


## Design Pattern 3: Chain of Responsibility

### Problem: 
This is used when you want to decouple a request and a reciever by giving several objects a chance to fufill the request.

### Solution:
Create a chain of objects that attempt to handle the requests in order, until one of them actually handles it.

### Consequences: 
* Decouples object and the handler since it does not know which class is the one handling the function. It only knows that the function i shandled
* Adds flexibility in assigning responsiblities
* Receipt isn't guaranteed - the request may go through the entire chain and not be handled
