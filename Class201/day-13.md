# Local Storage: The Past, Present, & Future of Local Storage for Web Apps
* Native client applications have the advantage over web applications because of local storage
* When native apps need storage you can embed your own database, invent your own file, or a number of other solutions
* Cookies were invented for web apps but they had some issues
  * Cookies are included in every HTTP request, slowing down your web app by transmitting the same data over and over
  * Sending data unencrypted over the internet
  * Limited to 4 KB of data - enough to slow down your app but not enough to be very useful

## HTML5 Storage - Web Storage
* A way for web pages to store named key/value pairs locally, within the client web browser
* Data stays even after you navigate away from the web site, close your browser tab, ect
* Unlike cookies, this data is never transmitted to the remote web server (unless you choose to send it)
* Implemented natively in web browsers so no plugin is needed
* From your JavaScript you can access HTML5 Storage through the `localStorage` object on your global window object

`function supports_html5_storage() {

  try {
  
    return 'localStorage' in window && window['localStorage'] !== null;
    
    } catch (e) {
    
      return false;
      
    }
    
  }`
* Modernizr can be used to detect support for HTML5 storage
`if(Modernizr.local) {

  // window.localStorage is available!
  
  } else {
  
   // no native support for HTML5 storage : (
   
   // maybe try dojox.storage or a third-party solution
   
  }`
  
  ## Using HTML5 Storage
  * HTML5 Storage is a key/value pair system
    * Store data based on a named key
    * Retrieve that data with the same key
    * Key value is always a string - data can be any type of JavaScript
    * Data is stored as a string so you need to use `parseInt()`, `parseFlaot()` ect
  * Methods
    * `setItem()` - will silently overwrite the previous value
    * `getItem()` - will return null if called on a non-existent key
    * `removeItem()` - will remove the value for the given key
  * You can keep track of whens storage area changes with the *storage* event

## Storage-Event Object
| Property | Type | Description |
|----------|------|-------------|
| `key` | string | the named key that was added, removed, or modified |
| `oldValue` | any | the previous value (now overwritten), or null if a new item was added |
| `newValue` | any | the new value, or null if an item was removed |
| `url*` | string | the page which called a method that triggered this change |
