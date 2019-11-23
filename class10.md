## 11/23/19

## JS Debugging

### Execution Contexts

Every statement in js lives in one of three execution contexts: 

- **Global Context** | code that is in the script, but not in a function.There is only one global context in any page
- **Function Context** | code that is being run within a function. Each function has its own function context
- **Eval Context** | text is executed like code in an internal function called `eval()`.

_global contexts_ correspond with a _global scope_. This means that, if the variable is declared outside a function, it can be used anywhere because it has this scope.

_function contexts_ correspond with a _function-level scope_. This means, when the variable is declared within a function, it can only be used within that function.

### The Stack and Hoisting

Each time a script enters a new execution context, there are two phases of activity:

1. **Prepare** 
    - The new scope is created
    - Variables, functions, and arguments are created
    - The value of the `this` keyword is determined
2. **Execute**
    - Now it can assign value to variables
    - Reference functions and run their code
    - Execute statements

It also creates a **variables object**, which contains details of all the variables.


### Errors

There is a list of errors and what what they mean on page 460 of our book.

### Debugging

You can narrow down what the problem might by following this workflow:
1. Where is the problem? 
    - Look at the error message
    - Check how far the script is running
    - Use breakpoints where things are going wrong.
2. What exactly is the problem?
    - When you have set breakpoints, you can see if the variables around them have the values you would expect them to
    - Break down/break out parts of the code to test smaller places of the functionality
    - Check the number of parameters for a function, or the number of items in an array

Resources:
- console
- `console.log`
- `typeof`
- linter
- follow the variable
- commenting out code
- break points

#### [Back to Home](index.md)