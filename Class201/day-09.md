# Forms (p144-175)
## Form Controls
* Adding Text:
  * Text Input
  * Password Input
  * Text Area
* Making Choices:
  * Radio Buttons
  * Checkboxes
  * Drop-down boxrs
* Submitting Forms
  * Submit buttons
  * Image Buttons
  * Uploading Files

## How Forms Work
1. User fills in a form and presses a button to submit info to the server
2. Name of each form control is sent to the server with the value the user enters/selects
3. Server processes info and may store info in a database
4. Server creates a new page to send back to the browser based on recieved info

## Form Structure
* Form controls live inside a &lt;form&gt; element
  * Should always carry an action="" attribute
    * Contains a url for the page on the server that will recieve the form info
  * Usually have a method and id attribute
    * get method: for short forms and search boxes
    * post method: for uploading files, sensitive data(passwords), or adding/deleting data from database
  * id: used to identify the form from other elements on the page

### Text Input
&lt;input type="text" name="username" size="15" maxlength="30" /&gt;
* name: value of this attribute identifies the form control and is sent along with info to the server
* maxlength: used to limit number of characters in a textfield (EX: year)

### Password Input
&lt;input type="password" name="" size="15" maxlength="30" /&gt;

### Text Area
&lt;textarea name="comments" cols="20" rows="4" &gt; *Enter your commments* &lt;/textarea&gt;

### Radio Button
&lt;input type="radio" name="genre" value="rock" checked="checked" /&gt;
* You will have multiple of these buttons but only one will contain checked

### Checkbox 
&lt; type="checkbox" name="service" value="itunes" checked="checked" /&gt;
* Same as radio button

### Drop Down List
    &lt;select name=""&gt;
    &lt;option value=""&gt;&lt;/option&gt;
    &lt;/select&gt;
* Create a tag for each option

### File Input Box
    &lt;input type="file" name="" /&gt;
    &lt;input type="submit" name="" value"" /&gt;
    
### Submit Button
&lt;input type="submit" name="" value"" /&gt;

### Image Button
&lt;input type="image" src="" width="" height="" /&gt;

# List, Tables, & Forms (p330-357)
## CSS List Styles
* unordered lists
  * none
  * disc
  * circle
  * square
* ordered lists
  * decimal: 1, 2, 3
  * decimal-leading-zero: 01, 02, 03
  * lower-alpha: a, b, c
  * upper-alpha: A, B, C
  * lower-roman: i. ii. iii.
  * upper-roman: I. II. III.

# Events (p243-292)
* Events happen when a user clicks on a link, hovers/swipes over an element, types on a keyboard, resize their window, or when the page loads

## Event Types
* UI Events
  * load: web page has finished loading
  * unload: web page is unloading ( usually because a new page is requested
  * error: browser encounters a JS error or an asset doesn't exist
  * scroll: user has scrolled up/down the page
* Keyboard Events
  * keydown: user first presses a key (repeats while key is depressed)
  * keyup: user releases key
  * keypress: character is being inserted
* Mouse Events
  * click: user presses and releases a button over the same element
  * dblclick: user presses and releases a button twice over the same element
  * mousedown: user presses a mouse button while over an element
  * mouseup: user releases a mouse button while over an element
  * mousemove: user moves the mouse (Not on touchscreen)
  * mouseover: user moves the mouse over an element
  * mouseout: user moves the mouse off an element
* Focus Events
  * focus/focusin: element gains focus
  * blur/focusout: element loses focus
* Form Events
  * input: value in any &lt;input&gt; or &lt;textarea&gt; element has changed or any element with the contenteditble attribute
  * change: value in select box, checkbox, or radio button changes
  * submit: user submits a form
  * reset: user clicks on a form's reset button
  * cut: user cuts content from a form field
  * copy: user copies content from a form field
  * past: user pastes content into a form field
  * user selects some text in a form field

