# Layout (p360-402)
## CSS Positioning
### Relative Positioning
* Shifts the element to the Top, Right, Bottom, or Left of the normal positioning
* top, bottom, left, and right are used to indicate how far the element is from its normal flow position

Written like -
    
    position: relative;
    top: 20px;
    left 200px;
### Absolute Positioning
* Positions element in relatoin to its containing element. 
* Takes it out of normal flow meaning that it does not affect the position of other elements on the page
* top, bottom, left, and right are used to indicate where the element should appear in relation to its containing element

Written like -

    position: absolue;
    top: 20px;
    left 100px;
    
### Fixed Positioning
* Positions element in relation to the browser window
* top, bottom, left, and right to indicate where the fixed position box will appear in relation to the browser window

Written like - 

    position: fixed;
    top: 10px;
    left: 0px;
    
### Z-Index
* WHen using relative, fixed, or absolute positoining these boxes can overlap, the z-index property controls which elements sit on top
* Its captured by a number/int
* The higher the value, the closer to the top that element will be

Written like -

      z-index: 15;
      
 ### Floating Elements
 Takes the element out of normal position and moves it to the left or right of the screen
 
 Written like -
 
      float: right;
      float: left;
      
### Clearing Float
Allows you to say that no element (within the same containing element) should touch the left or right-hand sides of the box

Written like -

      clear: left;
      clear: right;
      clear: both;
      clear: none;
      
## Screen Size and Resolution
Due to the countless screen sizes and resolution, web designers often create pages between 960-1000 pixels wide
## Page Layouts
### Fixed Width Layouts
* do not change size as the user increase or decreases the size of their browser (typically in pixels)
  * Advantages
    * Pixel values are accurate
    * Designer has more control over appearnce and position
    * You can control the lengths of the lines of texts
    * Image size will remain the same relative to the rest of the page
  * Disadvantages
