# Problem Domain, Objects, and the DOM
## Object Literals (p100-105)
Objects group together variables and functions and give them new names
* Variables become known as properties
  * Tell us about the object
* Functions become known as methods
  * Represent the task that is associated with the object

### Creating an Object Literal
var = hotel {
  name : 'Quay',
  rooms : 40,
  booked : 20,
  checkAvailability : function() {
    return this.rooms - this.booked;
  }
}
#### Accessing an object
var hotelName = hotel.name; object['property name']
var roomsFree = hotel.checkAvailability(); object['method name']();

## Document Object Model (p183-242)
The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JS can access/update the content of a web page.

DOM tree is the model structure
Consists of 4 node types:
* Document
* Element
* Attribute
* Text

### Accessing a DOM tree
* Locate node that represents the element you want
  * getElementByID()
  * getElementByClassName()
  * parentNode
* Use its text content, child elements, and attributes
* Accessing elements ( goes in parentheses of the function/method)
  * ID
  * CSS selector
  * Class
  * tagName

### NodeList
DOM queries that return more than one element
Selecting elements from NodeList
* item()METHOD
* Array Syntax

### Traversing the DOM
* parentNode
* previousSibling/nextSibling
* firstChild/lastChild

### Adding to DOM
* createElement()
* createTextNode()
* appendChild()

### Remocing Element from DOM 
* removeEl
* removeChild()
