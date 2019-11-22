## 11/23/19

## JS Debugging

### Execution Contexts

Every statement in js lives in one of three execution contexts: 

- **Global Context** | code that is in the script, but not in a function.There is only one global context in any page
- **Function Context** | code that is being run within a function. Each function has its own function context
- **Eval Context** | text is executed like code in an internal function called `eval()`.

_global contexts_ correspond with a _global scope_. This means that, if the variable is declared outside a function, it can be used anywhere because it has this scope.

_function contexts_ correspond with a _function-level scope_. This means, when the variable is declared within a function, it can only be used within that function.

### The Stack




#### [Back to Home](index.md)