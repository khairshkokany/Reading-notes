# JS
## WHAT IS AN OBJECT?
### Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.
## creating an object : leiteral notation.

### literal notation is the rasiest and most popular way to create objects.

## accessing an object and dot notation
* you access the properties or methods of an object using dot natation.
* you can also access properties using square brackets.
## docment object model
### WORKING WITH THE DOM TREE 


> Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 

1. STEP 1: ACCESS THE ELEMENTS
* SELECT AN INDIVIDUAL ELEMENT NODE
* SELECT MULTIPLE ELEMENTS (NODELISTS) 
* TRAVERSING BETWEEN ELEMENT NODES

2. WORK WITH THOSE ELEMENTS
 * ACCESS/ UPDATE
TEXT NODES 
* WORK W ITH HTML
CONTENT 
* ACCESS OR UPDATE
ATTRIBUTE VALUES 

## ACCESSING ELEMENTS 
### DOM queries may return one element, or they may return a Nodelist,which is a collection of nodes. 
### SELECT ELEMENTS
1. SELECTING ELEMENTS
USING ID ATTRIBUTES
2. SELECTING ELEMENTS
USING class ATTRIBUTES
3. SELECTING ELEMENTS
BY TAG NAME
4. SELECTING ELEMENTS
USING CSS SELECTORS 

### TRAVERSING THE DOM 
1. parentNode
2. previousSibling
nextSibling 
3. firstChild and
lastChild 

### HOW TO GET/UPDATE ELEMENT CONTENT 

#### So far this chapter has focused on finding elements in the DOM tree. 
#### The rest of this chapter shows how to access/update element content.
#### Your choice of techniques depends upon what the element contains. 

## ACCESS & UPDATE A TEXT NODE WITH NODEVALUE
### When you select a text node, you can retrieve or amend the content of it using the node Va 1 ue property

## ACCESSING & CHANGING A TEXT NODE
## ACCESS & UPDATE TEXT WITH TEXTCONTENT (& INN ERTEXT)

## ACCESSING TEXT ONLY 
## ACCESS & UPDATE TEXT & MARKUP WITH INNERHTML
### Using the i nnerHTML property, you can access and amend the contents of an element,including any child elements. 

## ADDING ELEMENTS USING DOM MANIPULATION
1. CREATE THE ELEMENT
2. GIVE IT CONTENT 
3. ADD IT TO THE DOM 
## REMOVING ELEMENTS VIA DOM MANIPULATION 
1. STORE THE ELEMENT
TO BE REMOVED IN A
VARIABLE 
2. STORE THE PARENT OF
THAT ELEMENT IN A
VARIABLE
3. REMOVE THE ELEMENT
FROM ITS CONTA INING
ELEMENT
 ## COMPARING TECHNIQUES:UPDATING HTML CONTENT
 1. document.write() 
 2. element.innerHTML