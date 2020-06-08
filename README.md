# CSS Position

 - **static** : This is the default value.
    It will come sequencially 
 - **relative** : RELATIVE ALMOST SAME AS STATIC BUT IT HAS OPTION TO MOVE LEFT, RIGHT, TOP, BOTTOM. . IT DOES OVERFLOW THAT REMOVE FROM DOCUMENT FLOW

 `position: relative;left: 100px;`

 relative to itself based on the values of top, right, bottom, and left. *it works exactly as static position*  It Allows to do 4 thing can't done by static that is ***top, bottom, left, right***
 
 - **absolute** : IT'S COMPLETLY REMOVED FROM DOCUMENT FLOW AND UNLIKE RELATIVE IT MOVE TOM, BOTTOM, LEFT, RIGHT FROM THE VERY BEGANNING OF THE SCREEN THAT MEANS START FROM X AXIS 0 AND Y AXIS 0. AND IF I SET PARENT ELEMENT POSITION RELATIVE IT WILL START FROM TOP BEGANNING OF PARENT  AND LEFT BEGANNING OF PARENT.


 ```
position: absolute;
left: 0;
top: 0;
 ```
 
 no space is created for the element in the page layout. It is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial containing block. Its final position is determined by the values of top, right, bottom, and left.
 
 - **fixed** : IT ALMOST SAME AS ABSOLUTE. IT NOTHING TO DO WITH PARENT. WORK WITH ENTIRE HTML. STAY IN THE SAME PLACE 

 ```
position: fixed;
left: 0;
 ```

 It is positioned relative to the initial containing block established by the viewport
 - **sticky** : relative to its nearest scrolling ancestor and containing block (nearest block-level ancestor), including table-related elements, based on the values of top, right, bottom, and left. The offset does not affect the position of any other elements.


 # SASS

direct scss file will not work with html we need to compile .
There is two main way to compile it to css

 1. by using npm package 

 ```
 npm install -g sass
 sass --watch scss/style.scss css/style.css
 ```

 2. use a extension in vsc name **live sass compiler**