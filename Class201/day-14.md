# CSS Transforms, Transitions, Animations
## CSS Transforms
* CSS3 has new ways to position/alter elements
  * These can be utilized with the `transform` property
  * Trasnform comes with two settings: 2D and 3D

Examples:
* 2D Rotate: rotates an element from 0 to 360 degrees
  * Positive value will rotate element clockwise
  * Negative value will rotate element counterclockwise

`transform: rotate(20deg);`

* 2D Scale: changes the size of the element
  * Default scale value is 1
    * Any value from .99-.01 makes the element smaller
    * Any value >= 1.01 makes the element bigger
  * `scaleX` and `scaleY` allow you to scale just x or y
  * `scale(x,y);` to scale each axis separately.

`transform: scale(.75);`

* 2D Translate: changes the position of the element without interrupting the normal flow
  * handled similar to Scale

`transform: translate(-10px, 25%);`

* 2D Skew: used to distort elements on the horizontal and vertical axis
  * handled similar to Scale and Translate

`transform: skew(5deg, -20deg);`

* Combining Transforms
  * List transform values within the transform property one after another without the use of commas
  * Using multiple transform declarations will not work as they override eachother

`transform: skew(10def, 20deg) translateX(20px);`

* Transform Origin: Changes default origin position 
  * Default is 50% horizontally and 50% vertically
  * `0,0` is the same as `top left`
  * `100%,100%` is the same as`bottom right`

`transform-origin: top left;`

* Perspective:
  * In order for 3D transforms to work the element needs a perpective to transform
  * Can be used within the transform property of the element
  * Can be used within the property on the parent element

`transform: perspective(200px) rotateX(45deg);`

## CSS Transitions and Animations
* Transitions: provide a change from one state to another
  * `:hover` or `:focus` or `:active` or `:target` psuedo-classes
  * `transition-property` or `transition-duration` or `transition-timing-function` or `transition-delay` 

`trasition-property: background;`

`transition-duration: 1s;`

`transition-timing-function: linear;`

* Animations: Build visiual interactions from one state to another
  * use @keyframes to set multiple points at which an element should undergo transition
    * @keyframes includes
      * animation name
      * any animation breakpoints
      * properties intended to be animated

`@keyframes slide {`

  `0% {`
  
    `left: 0;`
    
    `top: 0;`
    
  `}`
  
  `50% {`
  
    `left:244px;`
    
    `top: 100px;`
    
  `}`
  
  `100% {`
  
    `left: 488px;`
    
    `top: 0;`
    
  `}`
  
`}`


