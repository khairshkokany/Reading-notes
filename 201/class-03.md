# HTML 
## LISTS 
### ordered lists 
    <ol>
    The ordered list is created with the   <ol> element.
    <li>
Each item in the list is placed
between an opening < li> tag
and a closing  < /li> tag. 
(The li stands for list item.)
> this is will be a number list . 

### Unordered Lists

< ul>
The unordered list is created
with the < ul> element.
< li>
Each item in the list is placed
between an opening < i> tag
and a closing </ li> tag. (The li
stands for list item.)
> this is will be bullet point . 

### Definition lists

< dl>
The definition list is created with
the < dl> element and usually
consists of a series of terms and
their definitions.
Inside the < dl> element you will
usually see pairs of < dt> and
< dd> elements.
< dt>
This is used to contain the term
being defined (the definition
term).
< dd>
This is used to contain the
definition.

### Nested Lists

You can put a second list inside
an < li> element to create a sublist or nested list.
Browsers display nested lists
indented further than the parent
list. In nested unordered lists,
the browser will usually change
the style of the bullet point too.

> it will be a list inside list but the 2nd list will be for example open circle to know a diffrence between main point and the other lists. 
# CSS 
## BOXES
### BOX DIMENTIONS
#### width , height 

**By default a box is sized just big enough to hold its contents.**
**To set your own dimensions for a box you can use the height and width properties.**

> this is example of css 

div.box {
height: 300px;
width: 300px;
background-color: #bbbbaa;}
p {
height: 75%;
width: 75%;
background-color: #0088dd;}

> we will changed the size, background color of div and p . 

### Limiting Width
#### min-width, max-width

**Some page designs expand and shrink to fit the size of the user's screen.**
*** In such designs, the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.**

**These are very helpful properties to ensure that the content of pages are legible (especially onthe smaller screens of handheld devices).**
> For example, you can use the max-width property to ensure that lines of text do not appear too wide within a big browser window and you can use the min-width propertyto make sure that they do not appear too narrow. You may find it helpful to try this example out in your browser so that you can see what happens when you increase or decrease the size of the browser window.

### Limiting Height
#### min-height, max-height

**In the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it.**

**This isachieved using the min-height and max-height properties.**

> The example on this page demonstrates these properties in action It also shows you what happens when the content of the box takes up more space than the size specified for the box If the box is not big enough to hold the content, and the content expands outside the box it can look very mess,To control what happens when there is not enough space for the content of,a box, you can use the overflow property, which is discussed on the next page.

### Overflowing Content
#### overflow

**The overflow property tells the browser what to do if the conten contained within a box is larger than the box itself It can have one of two values.**

#### hidden 
**This property simply hides any extra content that does not fit in the box.**

#### scroll
**This property adds a scrollbar to the box so that users can scroll to see the missing content.**


## Border, Margin & Padding

**this is img will explain them.**

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Css_box_model.svg/640px-Css_box_model.svg.png" alt=border,margin,padding width=250px>

# JS 
## if statments 
* Use if to specify a block of code to be executed, if a specified condition is true.
* Use else to specify a block of code to be executed, if the same condition is false.
* Use else if to specify a new condition .to test, if the first condition is false
* Use switch to specify many alternative blocks of code to be executed.


***[this is example of if statments ..!](https://www.w3schools.com/js/js_if_else.asp)***


## switch statments 
* The switch expression is evaluated once.

* The value of the expression is compared with the values of each case.

* If there is a match, the associated block of code is executed.

* If there is no match, the default code block is executed.

***[this is example of switch statments ..!](https://www.w3schools.com/js/js_switch.asp)***

## TYPE COERCION & WEAK TYPING

DATA TYPE |PURPOSE
----------|------------------------------
string    |Text
number    |Number
Boolean   | true or false
null      | Empty value
undefined | Variable has been declared but not yet assigned a value

## loops

### WHILE & DO LOOPS 

**The do/while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.**

***[this is example of while & DO loops ..!](https://www.w3schools.com/js/js_loop_while.asp)***
