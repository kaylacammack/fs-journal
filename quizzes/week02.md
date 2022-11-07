# Intro to JavaScript

**1.** Which keywords are used to declare a variable in JavaScript?

<!-- enter you answer in the space below -->

```
var (antiquated now), let, and const
```

**2.** What is the definition of a function?

<!-- enter you answer in the space below -->

```
A function is a subprogram designed to perform a particular task.
```

**3.** What are the `SOLID` principles?

<!-- enter you answer in the space below -->

```
S - Single Responsibility Principle - a class should have only one reason to change or one job.
O - Open-Closed Principle - Functions should be open for extension (being able to add new features or components without breaking existing code) but closed for modification (we should not introduce breaking changes to existing functionality)
L - Liskov-Substitution Principle - a subclass should override the parent class methods in a way that does not break functionality from a client's point of view.
I - Interface Segregation Principle - a client shouldn't be forced to depend on methods they do not use.
D - Dependency Inversion Principle - entities must depend on abstractions not on concretions. It states that the high level module must not depend on the low level module, but depend on abstractions.
```

**4.** Given this array:

```js
let fruit = ["apple", "banana", "pineapple", "orange", "strawberry"];
```

What index is the pineapple's current position? How do you know?

<!-- enter you answer in the space below -->

```
2. The array starts at 0, so apple would be 0, banana would be 1, and pineapple would be 2.
```

**5.** With these two objects:

```js
let you = { name: "You", hair: true, friends: [] };
let them = { name: "Them", hair: false, friends: [] };
```

how would you .push the `them` object into the `you` object's array of friends?

<!-- enter you answer in the space below -->

```
you.friends.push(them);
```

**6.** Give an example of a JavaScript `Conditional`:

<!-- enter you answer in the space below -->

```
if(condition){
    block of code to be executed if condition is true
}
```

**7.** In the `for loop` below, what is the name of the piece belongs inside the empty "**\_\_**" space? What would you put here to increase `i` by one on every iteration?

```js
for ( let i = 0; i < arr.length; _______ ) {
  //...
```

<!-- enter you answer in the space below -->

```
If I understand correctly, after the // The name of the piece belonging in the curly brackets is the code block. Put i++ after arr.length to increase i by 1 on every iteration
```

**8.** What does the `DOM` acronym stand for? Which file is first accessed to render the `DOM`?

<!-- enter you answer in the space below -->

```
DOM stands for document object model. The index.html file is the first file accessed to render the DOM.
```

**9.** What are the `9` ECMAScript types as defined by MDN?

<!-- enter you answer in the space below -->

```
1. Null
2. Undefined
3. Boolean
4. Number
5. BigInt
6. String
7. Symbol
8. Objects
9. Properties
```

**10.** When it comes to functions or methods, what is the difference between a `parameter` and an `argument`?

<!-- enter you answer in the space below -->

```
When a value that is declared within a function when a function is invoked is an argument, whereas when a value is defined when a function is declared is called a parameter.
```

**11.** What is the difference between a `primitive` value and a `reference` value?

<!-- enter you answer in the space below -->

```
A primitive value is a value in-memory. A reference value refers to a value from a memory address (or a reference to a spot in memory).
```
