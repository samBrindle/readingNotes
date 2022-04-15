# JS Debuggin (Chapter 10)
## Order of Execution
* The order in which statements are exectued can be complex; some tasks cannot complete until another statement or function has been run

## Execution Contexts
* Every statement in a script lives in one of three execution contexts
  * Global Context: Code in the script but not in a function
  * Function Context: Code that is being run in an internal function
  * Eval Context: Text is executed like code in an internal function
* Variable Scope
  * Global Scope: If a variable is declared outside a function - Can be used anywere
  * Function-Level Scope: When a variable is declared in a function - Can only be used within that function

## Error Objects
* Can help you find where your mistakes are and browsers have tools to help you read them

### Error Properties
* Name: Type of execution
* Message: Description
* fileNumber: Name of JS file
* lineNumber: Line number of error

### Types of Error Objects
* Error: Generic error
* SyntaxError: Syntax has not been followed
* ReferenceError: Tried to reference a variable that is not declared/within scope
* TypeError: An unexpected data type that cannot be coerced
* RangeError: Numbers not in acceptable range
* URIError: encodeURI(), decodeURI(), and similar methods used incorrectly
* EvalError: eval() function used incorrectly

## Dealing with Errors
* Debug the script to fix errors
* Handle errors gracefullyr
