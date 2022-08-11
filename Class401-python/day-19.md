# Class 19 - Automation
## Python RegEx Tutorial
### Useful Regex Functions
* `import re`
* `compile()`
* `search()`
* `findall()`
* `sub()`
* `split()`

### Basic Paterns: Ordinary Characters
* You can use ordinary characters in simple regex:
  * `pattern = r"Cookie"`
  * will find check if the sequence matches the pattern exactly

### Character Table
| Character(s) | What it does |
|--------------|--------------|
| . | A period. Matches any single character except for newline |
| ^ | A caret. Matches a pattern at the start of a string |
| \A | Uppercase A. Matches only at the start of a string |
| $ | Dollar sign. Matches the end of the string |
| \Z | Uppercase Z. Matches only at the end of the string |
| [] | Matches the set of characters you specify within it |
| \ | Used to grab escape characters or treated like a normal character |
| \w | Lowercase w. Maches any single letter, digit, or underscore. |
| \W | Uppercase W. Matches any character not part of \w |
| \s | Lowercase s. Matches a single whitespace character like: space, newline, tab, return |
| \S | Uppercase S. Matches any character not part of \s |
| \d | Lowercae d. Matches decimal 0-9 |
| \D | Uppercase D. Matches any character that is not a decimal digit. |
| \t | Lowercase t. Matches tab |
| \n | Lowercase n. Matches newline |
| \r | Lowercase r. Matches return |
| \b | Lowervase b. Matches only the beginning or end of the word |
| + | Checks if the preceding character appears one or more times |
| * | Checks if the preceding character appears zero or more times |
| ? | Checks if the preceding character appears exactly zero or one time, specifies a non-greedy version of +,* |
| {} | Checks for an explicit number of times |
| () | Creates a group when performing matches |
| <> | Creates a named group when performing matches |
