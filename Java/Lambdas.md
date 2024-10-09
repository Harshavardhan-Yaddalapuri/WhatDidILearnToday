# What Are Lambda Expressions?

Lambda expressions are were introduced in Java 8 as a part of the Java language enhancments to support functional programming. They allow you to pass behavior (code) as a parameter to methods, which makes your code more flexible and concise.

## 1. Key Characteristics of Lambda Experssions

- **[Functional Interface](https://www.geeksforgeeks.org/functional-interfaces-java/):** A lambda expression can only be used with a functional interface (an interface with a single abstract method). This allows for cleaner code, as you can express instances of functional interfaces more clearly.
- **Anonymous Function:** Lambda expressions are sometimes referred to as anonymous functions. They allow you to define functionality on-the-fly without needing to create a separate class.
- **Conciseness:** They significantly reduce the amount of boilerplate code compared to traditional anonymous class implementations.

## 2. Syntax Breakdown

The basic syntax of a lambda expression consists of three parts:

- **Parameter List:** This can be empty or contain one or more parameters. Types can often be inferred, allowing for a simplified syntax.
- **Arrow Token(->) :** This separates the parameter list from the body of the lambda.
- **Body:** This can be a single expression or a block of code enclosed in curly braces. If it’s a single expression, the return type is inferred, and no return statement is needed.

### Examples for different lambda implementations:

1. No Parameters:

```java
() -> System.out.println("Hello, World!")
```

2. Single Parameter (Type Inferred):

```java
name -> System.out.println(name)
```

3. Multiple Parameter:

```java
(a, b) -> a + b
```

4. Single Statement: (Implicit Return):

```java
(x) -> x * x // Returns the square of x
```

5. Multiple Statements (Explicit Return):

```java
(x) -> {
    int square = x * x;
    return square;
}

```

## 3. Benifits of Using Lambda Expressions

- **Readability:** Code becomes more readable and easier to understand. Functional constructs often express intent more clearly than traditional coding methods.

- **Less Boilerplate Code:** You reduce the amount of code you write. For example, with lambda expressions, you don't need to create a new class just to implement a single method.

- **Encourages Functional Programming:** They promote a functional programming style, making it easier to write higher-order functions (functions that take other functions as parameters or return them).

- **Better Support for APIs:** Many Java APIs, especially those dealing with collections (like the Stream API), are designed to work with lambda expressions, making operations like filtering, mapping, and reducing data collections much more straightforward.

## 4. When to use?

- **Collections Framework:** Use lambdas with the forEach, map, filter, and reduce methods available in the Java Collections Framework, particularly with Streams.

- **Event Handling:** Lambdas are commonly used in GUI frameworks (like JavaFX or Swing) for event handling, allowing you to specify what happens when an event occurs without the need for verbose inner classes.

- **Threading:** You can use lambdas to implement Runnable or Callable without the boilerplate of creating a new class.
