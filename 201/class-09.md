# HTML 

## LISTS, TABLES AND FORMS


* Specifying bullet point styles.
* Adding borders and backgrounds to tables
* Changing the appearance of form elements
> There are several CSS properties that were created to work with specific types of HTML elements, such as lists, tables, and forms.

we will learn how to:

* Specify the type of bullet point or numbering on lists
* Add borders and backgrounds to table cells
* Control the appearance of form controls
> Together, these properties allow you to take finer control over specific parts of your pages.

### BULLET POINT STYLES

**he list-style-type property allows you to control the shape or style of a bullet point (also known as a marker).**

**It can be used on rules that apply to the < ol>, < ul>, and < li> elements.**

> Example :- 


<img src = "https://www.oreilly.com/library/view/html-css/9781118206911/images/ch014-Uf002.jpg" width = 250px>
<img src = "https://www.oreilly.com/library/view/html-css/9781118206911/images/ch014-Uf003.jpg" width = 250px>
<img src = "https://www.oreilly.com/library/view/html-css/9781118206911/images/ch014-Uf004.jpg" width = 250px>

### UNORDERED LISTS

**For an unordered list you can use the following values:**

* none
* • disc
* circle
* square

### ORDERED LISTS
**An ordered list starts with the < ol> tag. Each list item starts with the < li> tag.** 

* type="1"	The list items will be numbered with numbers (default)
* type="A"	The list items will be numbered with uppercase letters
* type="a"	The list items will be numbered with lowercase letters
* type="I"	The list items will be numbered with uppercase roman numbers
* type="i"	The list items will be numbered with lowercase roman numbers


## HTML FORMS 

### The <form> Element
* The HTML < form> element is used to create an HTML form for user input:

> The < form> element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.
> All the different form elements are covered in this chapter: HTML Form Elements.


### The < input> Element

* The HTML < input> element is the most used form element.

* An < input> element can be displayed in many ways, depending on the type attribute.


> Example 


Type	Description
1. < input type="text">  	Displays a single-line text input field
2. < input type="radio">	Displays a radio button (for selecting one of many choices)
3. < input type="checkbox">	Displays a checkbox (for selecting zero or more of many choices)
4. < input type="submit">	Displays a submit button (for submitting the form)
5. input type="button">	Displays a clickable button

# JS

## Events

**HTML events are "things" that happen to HTML elements.**

**When JavaScript is used in HTML pages, JavaScript can "react" on these events.**

### HTML Events
> An HTML event can be something the browser does, or something a user does.

> Here are some examples of HTML events:

* An HTML web page has finished loading
* An HTML input field was changed
* An HTML button was clicked
> Often, when events happen, you may want to do something.

* JavaScript lets you execute code when events are detected.

> HTML allows event handler attributes, with JavaScript code, to be added to HTML elements.


***What can JavaScript Do?***
**Event handlers can be used to handle and verify user input, user actions, and browser actions:**

1. Things that should be done every time a page loads
2. Things that should be done when the page is closed
3. Action that should be performed when a user clicks a button
4. Content that should be verified when a user inputs data
6. And more ...

> Many different methods can be used to let JavaScript work with events:

1. HTML event attributes can execute JavaScript code directly
2. HTML event attributes can call JavaScript functions
3. You can assign your own event handler functions to HTML elements
4. You can prevent events from being sent or being handled
5. And more ...