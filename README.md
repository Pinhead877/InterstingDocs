# Stuff to learn

- How to wait for a thread
- When to use a finalizer
- Boxing unboxing - why is it so expensive to use.
- Check the parameter in ConfigureAwait - continueOnCapturedContext
- Threads join - what's is it, how to use it and when to use it?

# Multithreading

## Tasks

- Task wraps the thread and thread pool classes.
- Task can return a result.
- Thread can&#39;t return a result.
- In order to wait for a thread to complete we need to use signaling events like AuthoResetEvent and ManualResetEvet
- A task can become a parent task of other tasks. This means that the parent task wont complete until the child tasks are completed.
- Exception in the children tasks are handled with the AggregateException which holds all of the errors from the other child tasks.

## Interlocking Functions

- A class that provides methods to perform thread safe manipulation on variables of integer.
- For example, if two concurrent thread will try to update the same integer they can override the value of each other.

# Design Patterns

You should use design patterns to make your code more flexible and the code more reusable.

## Creational Patterns

### Factory Method

- Uses a CreateMethod to initialize the object. This happens in the concrete class of the specific type.
- Separates the creation of the object from its use in the code. The use of the object in the code will be handled through an interface. This interface will declare the methods that are used in the code.
- This design could be used to extend the library or framework that you are writing. Just inherit the type and the framework you want to extend and write minimal code for the job.

| Pros | Cons |
| --- | --- |
| Object create and use are separated | can make the code very complicated if the we will have a lot of subclasses of the creators. |
| Single responsibility |   |
| Open/closed principle \*  – we can add new types to the code without breaking the code. |   |
