# FileIO & Exceptions
## Read & Write in Python
* Opening a file in Python
  *  `open('filename.txt', 'mode')`
* Three different categories of files
  * Text files - opened using the open() method
  * Buffered Binary Files - opened with modes `rb` (read binary) or `wb` (write binary)
  * Raw Files - opened with `rb, buffering=0`
 
 ## Exceptions in Python
 * Python programs terminate when they hit syntax errors or exeption errors
 * Use the `raise` method to throw an expection under a specific circumstance wih a custom message
 * Assertions allow you to create a truthy evaluation where the code will continue if truthy but throw AssertionError if falsy
