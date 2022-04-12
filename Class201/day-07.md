## Tables (p126-145)
Tables represent information in a grid format
### Table Structure
| Tag | Name | Info |
|-----|------|------|
| &lt;table&gt; | table | creates a table |
| &lt;tr&gt; | table row | creates a new row |
| &lt;td&gt; | table data | information in a table cell |
| &lt;th&gt; | table header | used to name a row/column |
| &lt;th scope='col'&gt; | scope | column header |
| &lt;th scope='row'&gt; | scope | row header |
| &lt;td colspan='#'&gt; or &lt;th colspan='#'&gt;| column span | streteches entries across multiple columns, # indicates # of columns |
| &lt;td rowspan='#'&gt; or &lt;th rowspan='#'&gt; | row span | stretches entries across multiple rows, # indicates # of rows |

### Long Table Structure
| Tag | Name | Info |
|-----|------|------|
| &lt;thead&gt; | headings | used to store every heading of the table |
| &lt;tbody&gt; | body | body of table |
| &lt;tfoot&gt; | footer | table footer |

## Functions, Methods, and Objects (p106-144)
### Creating an object: Constructor Notation
* Use "new" keyword and the object constructor to create an empty object
* You can add properties and methods to the object

### Updating an object
* Using dot notation
  * hotel.name = 'park';

### Creating many objects: Constructor Notation
1. Use functions to template an object's properties and methods
2. Name the function using an uppercase letter 
3. Add parameters to function to set value of a property
4. Use "this" keyword to indicate property/method belongs to the object in **this** function

### Arrays and Objects
* Arrays can store a series of objects
* Objects can hold arrays

### Built in Objects
Browsers have 3 built-in objects:
* Browser Object Model
| Method | Info |
|--------|------|
| window.alert() | creates dialog box that user must click to close |
| window.open() | opens new browser window with url specified in parameter |
| window.print() | Tells browser user wants to print current page |

* Document Object Model (DOM)
| Method | Info |
|--------|------|
| document.write() | writes text to document |
| document.getElementId() | returns element if there is an element with the value of the id |
| document.querySelectorAll() | returns list of elements that match a CSS selector |
| document.createElement() | creates new element |
| document.createTextNode() | creates new text node |

* Global Javascript Objects
| Method | Info |
|--------|------|
| toUpperCase() | Changes string to uppercase |
| toLowerCase() | Changes string to lowercase |
| charAt() | takes an index number as a parameter and returns character found at that positon |
| indexOf() | returns index number of the first time a character is found within the string |
| lastIndexOf() | returns index number of the last time a character is found within the string |

