# UnderStanding Asynchronous Code, and API's

**1.** What is the difference between `asynchronous` code and `synchronous` code?

<!-- enter you answer in the space below -->

```
Asynchronous is when you can have your code continue running even when a request has been made. You create a callback or a promise for something to happen after that callback or promise is made, but your code still continues to run. Synchronous code will wait until the request has been resolved or rejected before proceeding to the rest of the code. This can result in poor user interface.
```

**2.** What is an event listener?

<!-- enter you answer in the space below -->

```
An event listener is a way that you can wait for user interaction and run code whenever that action happens. In class we have used it for when there is a change to the appState values to redraw the objects so that the user can see the updated objects.
```

**3.** What does the `O` represent in the `SOLID` principles?

<!-- enter you answer in the space below -->

```
The O represents the Open-Closed Principle which means software entities like classes, modules, and functions should be open for extension but closed for modification. A module is "open" if it is still available for extension, meaning you can add fields to the data structure it contains, or new elements to the set of functions it performs.
```

**4.** What is a callback / higher order function?

<!-- enter you answer in the space below -->

```
A callback is a function that is passed to another function. A higher order function takes another function as an argument and/or returns a function as a value.
```

**5.** What is a `promise`? How do you capture an error from a `promise`?

<!-- enter you answer in the space below -->

```
A promise is a guarantee that your request will be resolved. It is either successful or you get an error.
```

**6.** Name three processes used to make requests over `HTTP`?

<!-- enter you answer in the space below -->

```
Get, put, post, delete.
```

**7.** What does the `API` acronym stand for?

<!-- enter you answer in the space below -->

```
Application programming interface
```

**8.** In the `MVC` design pattern, who is responsible for making calls to `APIs`?

<!-- enter you answer in the space below -->

```
The service.
```

**9.** What is the purpose of encapsulation in programming?

<!-- enter you answer in the space below -->

```
Encapsulation restricts direct access to some components of an object.
```

**10.** What is `HTTP` response code for a successful request?

<!-- enter you answer in the space below -->

```
201
```

**11.** What is a 500 error?

<!-- enter you answer in the space below -->

```
Internal server error
```
