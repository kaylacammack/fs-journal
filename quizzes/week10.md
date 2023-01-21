# C# Fundamentals

**1.** What is the purpose of a `namespace`?

<!-- enter you answer in the space below -->

```
A namespace is used to organize code elements and create globally unique types.
```

**2.** What is the difference between a `class` and a `struct`?

<!-- enter you answer in the space below -->

```
A class is a data structure that combine data variables and functions into a single unit. Instances of the class are known as objects. Structures are light versions of classes.
```

**3.** What is the method that returns an instance of a class, yet it has no return type?

<!-- enter you answer in the space below -->

```
Void
```

## Example 1

```c#
abstract class Car
{
  ...
  public virtual string Start()
  {
    return "Vroooom";
  }
}
```

**5.** In the example what is the access modifier of the `Start()` method?

<!-- enter you answer in the space below -->

```
public
```

**6.** In the example what is `string` an indication of?

<!-- enter you answer in the space below -->

```
The type will be text.
```

**7.** In the example what is `abstract` preventing?

<!-- enter you answer in the space below -->

```
Hiding the car details
```

**8.** In the example what is the purpose of `virtual`?

<!-- enter you answer in the space below -->

```
To override the car class.
```

**9.** Name four access modifiers:

<!-- enter you answer in the space below -->

```
a. Public
b. Private
c. Protected
d. Internal
```

**10.** If you set a class or method to private, what can access it?

<!-- enter you answer in the space below -->

```
A private class or method can only be accessed from within the class.
```
