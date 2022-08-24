# Reading: Django CRUD and Forms
## Django Tutorial Part 9: Working with forms
### HTML Forms
* A collection of elements inside `<form>...</form>` tags
* Contain atleast one input element of `type='submit'`
* `action`: The resource/URL where data is being sent for processing on form submission
  * if this is not set the form will be submitted back to the current URL
* `method`: The HTTP method used to send the data
  * `POST`: used if the data is going to result in a change to the server's database because it is more resisitant to cross-site forgery attacks
  * `GET`: used for forms that don't change user data, such as a search form

### Django Form Handling Process
* View gets a request
* Performs any action required including reading data from the models
* generates and returns an HTML page

1. Display the default form the first time it is requested by user
2. Receive data from a submit request and bind it to the form
3. Clean and validate the data
4. If any data is invalid, re-display the form
5. If all data is valid, perform required actions
6. Once all actions are complete, redirect user to another page

#### Common arguments to most fields:
* `required`: If `True` cannot be left blank
* `label`: Label to use when rendering field in HTML
* `label_suffix`: Colon by default, can change to other characters
* `initial`: Initial value when the form is displayed
* `widget`: Display widget use
* `help_text`: Can be displaued in forms to explain field functionality
* `error_messages`: List of error messages for the field. Possible to override with your own messages
* `validators`: List of functions that will be called on the field when it is validated
* `localize`: Enables localization of form data input
* `disabled`: Prevents field from being edited if this is `True`
