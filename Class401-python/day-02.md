# Testing and Modules
## In Tests We Trust - TDD with Python
* Unit tests are some pieces of code to exercise the input, the ouput and the behaviour of your code
* Test-Driven Development is a strategy to think and write tests first

### Creating Tests
* Test Names: need to be descriptive about it and say what is expected and what is tested
* Test File Name: follow the same name of the module name
* Structure:
  *  Arrange: You need to organize the data neede to execute that piece of code(input)
  *  Act: Here you will execute the code being tested
  *  Assert: After executing the code, you will check if the result (output) is what was expected

## What does the if __name__ == "__main__": do?
* If we are running a module as the main program, its __name__ will be set to __main__
* If we are running a module from another file, it's __name__ will be se to __filename__.py
* Advantages:
  * Every Python module ahs it's __name__ defined, if it is __main__ it means the module is being run alone and we can do corresponding appropriate actions
  * If you import a script as a module in another script, the __name__ is set to the name of that script
  * Python files can act as reusable modules or standalone
  * If __name__ == "__main__": is used to execute some code only if the file is run directly

### What on Earth is Recursion?
* Recursion is the a process in which a function calls itself 
    * Performing the same operations multiple times with different inputs
    * In every step, we try smaller inputs to make the problem smaller
    * Base condition is needed to stop the recursion otherwise infinte loop will occur
