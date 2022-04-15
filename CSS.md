Q. how to add comments on css? A. /* */

Q. Why do we use pseudo-class? A. pseudo-class use to define special state of and element for exmple => style and element when mouses hover color changes like this => styled visited and unvisited links diffrence a:visited{ color: red } a:hover{ color:blue }

Q. How is specificity applied? A. let take a random example of specificity so when we write

Hello

in style we can write p{ color:green } #demo{ color:red } if we give particular class or id for that so our id is most powerfull so it's give output like what ever we want changes through id so final output will be red color will be happen
Q. What method allows an element to be moved from its current position? A. basiclly it's position property that allow move one postion to another position it's happen like that

static => that position not affected by the top, bottom, left, right
relative => it's adjacent anyway from it's normal postion
fixed => postion fixed that mean always stays in the same place even if the page is scrolled.
absolute =>it's uses the document body and moves alog with page scrolling.
sticky is bassed on user's scroll position
Q. what properties does flex model have? flex: flex-grow => how much the item will grow relative to the rest of the flexible items

flex-shrink=> the item will shrink relative to the rest of the flexible itmes

flex-basis|auto|initial|inherit;

Q. What is the difference between flex and grids? CSS grids are for 2D layouts. It works with both rows and columns. Flexbox works better in one dimension only (either rows OR columns). It will be more time saving and helpful if you use both at the same time.

Q. Give an example where we have to use grids and where you have to use flexbox? A. Grid can be used to create two dimensions layout B. flexbox can only be used to create one-dimensional layouts

Q. Give an example where you cannot use flexbox, and you can only use grids? A. when we have need to make 2D layouts that place we can not use flex only we can use grid.

Q. What are combinators? give examples of how you can use them A. A combinators is something that explains the relationship between the selectors

descendent selector(space)
child selector (>)
adjacent sibling selector(+)
general sibling selector(~)
Q. What does object-fit do? The object-fit property is used to specify how an  or

Q. What does rotate do? A. The transform property applies a 2D or 3D transformation to an elements this property allow you to rotate, scale, etc div.a{ transform: rotate(20deg); }

Q. What rule can be used to define animations A. @keyframes rule is used to define the properties that will be animated in an animation rule. div { width: 10px; height: 10px; background-color: red; animation-name: example; animation-duration: 40s; }

@keyframes example { from {background-color: red;} to {background-color: yellow;} }

Q. When working with attribute selectors, how can you select elements which contain a particular attribute value? A. The [attribute*="value"] selector is used to select elements whose attribute value contains a specified value.

[class*="te"] { background: yellow; }

Q. What does @media do? A. @media used in media queries to apply diffrent styles for different media types/devices.

Q. What can be used to override properties of an element? A. id and class is part of override properties in css

Q. How can you select every alternate elements in a list of elements using css? A. we can use :nth-child() selectors let we want to connect from div so div:nth-child(1){}, div:nth-child(3){} like that

Q. What is the ranking of selectors with respect to specificity A.

Inline style
ID
Class
Elements
Q. how can we apply same styles to multiple selectors? A. dive#main, div#sidebar { border:1px solid red; } p, .blue, #first, div span{ color : blue }