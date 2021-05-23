# About html 
**We will learn about HTML** 
**We will learn about CSS**
**We will learn about Practical** 
***How People Access the Web***
1. Browsers
2. Web Servers
3. Screen readers
4. Devices
***How Websites Are Created***
1. What you see
1. How it is Created
1. HTML5 & CSS3
***How the Web Works***
*When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.*
## Web page structure
The basic structure is in place; you simply need to change the title and add some text. The first thing we have to know is that in every web page there are two clearly differentiated parts: the head, or head, and the body, or body.
### This is example for html code :-
< html>
< body>
 < h1>This is the Main Heading</ h1>
 < p>This text might be an introduction to the rest of
 the page. And if the page is a long one it might
 be split up into several sub-headings.< p>
 < h2>This is a Sub-Heading</ h2>
 "< p>Many long articles have sub-headings so to help
 you follow the structure of what is being written.
 There may even be sub-sub-headings (or lower-level
 headings).< /p>"
 "< h2>Another Sub-Heading</ h2>"
 < p>Here you can see another sub-heading.</ p>
</ body>
</ html>
< h1>title</ h1>
< p>title             this is open tag of paragraph 
</ p>                   this is close tag of paragraph 


> To create a web page on a pc You can use a lot of programs like notepad , notepad ++ , VS .


### DOCTYPEs

Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included). We will therefore be including one in each example for the rest of the book. As you will see when we come to look at CSS and its box model on page 316, the use of a DOCTYPE can also help the browser to render a page correctly. Because XHTML was written in XML, you will sometimes see pages that use the XHTML strict DOCTYPE start with the optional XML declaration. Where this is used, it should be the first thing in a document. There must be nothing before it, not even a space.

#### Comments in HTML

If you want to add a comment
to your code that will not be
visible in the user's browser, you
can add the text between these
characters:
"<!-- comment goes here -->"

### ID Attribute

Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page.

Its value should start with a letter or an underscore (not a number or any other character).
It is important that no two elements on the same page have the same value for their id attributes (otherwise the value is no longer unique).
As you will see when you come to look at CSS in the next section, giving an element a unique identity allows you to style it differently than any other instance of the same element on the page.
< p id="pullquote">Every time I view the sea I feel
 a calming sense of security, as if visiting my
 ancestral home; I embark on a voyage of seeing.
</p>

### Class Attribute

Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page. For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements, or you might want to differentiate between links that point to other pages on your own site and links that point to external sites. To do this you can use the class attribute. Its value should describe the class it belongs to
< p class="important admittance">Hours: 10:00 – 18:00
 (No admittance after 17:30)</ p>

### Block Elements

Some elements will always appear to start on a new line in the browser window. These are known as block level elements.
Examples of block elements are

"< h1>, < p>, < ul>, and < li>."

### Inline Elements

Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements.
Examples of inline elements are
< a>, < b>, < em>, and < img>.

### HTML5 Layout Elements
< header> - Defines a header for a document or a section.
< nav> - Defines a set of navigation links.
< section> - Defines a section in a document.
< article> - Defines an independent, self-contained content.
< aside> - Defines content aside from the content (like a sidebar)

 ## process and design
Getting your message across using design
* Content 
* Prioritizing 
* Organizing 
* visual hierarchy :- 
1. Size
2. color
3. style 
* Grouping
1. Proximity
2. Closure
3. Continuance
* Similarity
1. White Space
2. color
3. Borders
* Designing Navigation
1. Concise
2. Clear
3. Selective
4. Context
5. Interactive
6. Consistent
## Introduction of java scripts 
### JavaScript is used for:
Adding interactive behavior to web pages. JavaScript allows users to interact with web pages. ...
* Creating web and mobile apps.
* Building web servers and developing server applications.
* Game development.
### Script 
A script is a series of instructions that the computer can follow in order to achieve a goal.
Each time the script runs, it might only use a subset of all the instructions.
Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically.
To approach writing a script, break down your goal into a series of tasks and then work out each step needed
to complete that task (a flowchart can help).

#### HOW A BROWSER SEES A WEB PAGE
1. RECEIVE A PAGE AS HTML CODE
2. CREATE A MODEL OF THE PAGE AND STORE IT IN MEMORY
3. USE A RENDERING ENGINE TO SHOW THE PAGE ON SCREEN
> And this is basic example of html , css & JS
<! DOCTYPE html>

< html >

< head>

< title>Constr ucti ve &amp ; Co.</ title>

< link rel ="stylesheet" href="css/cOl.css" />

< /head>

< body>

< hl>Constructive &amp ; Co.</ hl>

< p>For all orders and inquiries please call < em>555-3344</ em></ p>

= = < script src="j s/ add-content .j s "></ script>

</ body>

</ html>