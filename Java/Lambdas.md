# What Are Lambda Expressions?

Lambda expressions are were introduced in Java 8 as a part of the Java language enhancments to support functional programming. They allow you to pass behavior (code) as a parameter to methods, which makes your code more flexible and concise.

1. Key Characteristics of Lambda Experssions

- **[Functional Interface](https://www.geeksforgeeks.org/functional-interfaces-java/):** A lambda expression can only be used with a functional interface (an interface with a single abstract method). This allows for cleaner code, as you can express instances of functional interfaces more clearly.
- **Anonymous Function:** Lambda expressions are sometimes referred to as anonymous functions. They allow you to define functionality on-the-fly without needing to create a separate class.
- **Conciseness:** They significantly reduce the amount of boilerplate code compared to traditional anonymous class implementations.

2. Syntax Breakdown

The basic syntax of a lambda expression consists of three parts:

- **Parameter List:** This can be empty or contain one or more parameters. Types can often be inferred, allowing for a simplified syntax.
- **Arrow Token(->) :** This separates the parameter list from the body of the lambda.
- **Body:** This can be a single expression or a block of code enclosed in curly braces. If it’s a single expression, the return type is inferred, and no return statement is needed.
