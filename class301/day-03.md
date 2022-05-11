# Reading Notes Day 3: Passing Functions as Props
## Lists and Keys
### Rendering Multiple Components
* `.map()` loops through an array and returns elements for each item
### Keys
* key: special string attribute needed when creating lists of elements
* Help React identify which items have changed, were added, or were removed
* Give elements a stable identity
* Index could be used if there is no Key, but potential errors if order changes
* Keys must be unique among siblings
* Embed expression in curly brace so you can inline `.map()`

## How to Use the Spread Operator (...) in JavaScript
* Spread syntax refers to the use of an ellipsis (...) to expand an iterable object into the list of arguments
### What else can `...` do?
* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array

### The Spread Operator and Older Browsers
* The spread operator is not going to work on older Internet Explorer or older browsers

