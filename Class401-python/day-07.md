# Class 07 - Ten Thousand 2

## Python Scope & the LEGB Rule: Resolving Names in your Code
* LEGB - summarizes Python Scope levels and the sequence of steps Python follows when resolving names in a program
  * Local
  * Enclosing
  * Global
  * Built-in 

### Understanding Scope
* Scope - defines the area of a program in which you can unabiguously access that name
  * Global Scope: Names you define in this scopee are available to all of your code
  * Loacl Scope: Names you define in this scope are only available or visible within the scope

### Python Scope vs Namespace
* Namespace - Concrete mechanisms that Python uses to store names. Stored in a special attribute called .__dict__.
* Names at the top level of a module are stored in the module's namespace

### Using the LEGB Rule for Python Scope
* Local (function) scope - the code block or body of any Python function or lambda expression
  * These are created at function call not function creation
  * Each call creates a new scope
* Global (module) scope - The top-most scope in a Python program, script, or module
  * Contains all of the names you define at the top level of a program or a module
  * Visible from everywhere in your code
* Enclosing (nonlocal) scope - Special scope that only exists in nested functions
  * If local scope is an inner or nested function, then enclosing scope is the scope of the outer or enclosing function
* Built-in Scope - Special Python scope that is created or loaded whenever you run a script or open an interactive session

### Modifying the Behavior of a Python Scope
* Use the `global` tag to declare a variable as global in a function
* Use the `nonlocal` tag to use a non local variable in a nested situation

### Using Enclosing Scopes as Closures
* Closures - a special use case of the enclosing Python scope
   * When handling nested function data, statements that make up that function are packaged together with the environment 
