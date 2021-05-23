# Text in HTML 
## Headings
<h1>
<h2>
<h3>
<h4>
<h5>
<h6>
<h1> is used for main headings
<h2> is used for subheadings
<h6> this is the smallest one 
#### Example :- 
<h1>This is a Main Heading</h1>
## Paragraphs
***To create a paragraph, surround the words that make up the paragraph with an opening <p> tag and closing </p> tag***
#### Example :- 
<p>Text is easier to understand when it is split up  into units of text.</p>
## Bold & Italic
***By enclosing words in the tags and we can make characters appear bold.***
#### Example :- 
<b>key features</b>
## Superscript & Subscrip
<sup>
***The <sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power.***
#### Example :- 
4<sup>th</sup>
<sub>
***The <sub> element is used to contain characters that should be subscript. It is commonly
used with foot notes or chemical formulas.***
#### Example :- 
CO<sub>2</sub>.
## Line Breaks & Horizontal Rules 
<br /> 
***As you have already seen, the browser will automatically showeach new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag <br />.***
#### Example :- 
The Earth<br />
***<hr /> 
***To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the <hr /> tag.***
#### Example :- 
The Earth
<hr />
The other Earth 
## Strong & Emphasis
<strong> 
**The use of the <strong> element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis. By default, browsers will show the contents of a <strong> element in bold.**
#### Example :- 
<strong>Beware:</strong>
<em> 
*The <em> element indicates emphasis that subtly changes the meaning of a sentence. By default browsers will show the contents of an <em> element in italic*
#### Example :- 
<em>think</em>

## Quotations
<blockquote>
***The <blockquote> element is used for longer quotes that take up an entire paragraph. Note how the <p> element is still used inside the <blockquote> element. Browsers tend to indent the contents of the <blockquote> element, however you should not use this element just to indent a piece of text — rather you should achieve this effect using CSS.***

<q>
***The <q> element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the <q> element, however Internet Explorer does not — therefore many people avoid using the <q> element.***
#### Example :- 
<blockquote cite="http://en.wikipedia.org/wiki/Winnie-the-Pooh">  <p>Did you ever stop to think, and forget to start again?</p> </blockquote> <p>As A.A. Milne said, <q>Some people talk to animals. Not many listen though. That's the  problem.</q></p>
>And we have a lot of text we can use it .

# introudtion of CSS 
***CSS is the acronym of “Cascading Style Sheets”. CSS is a computer language for laying out and structuring web pages (HTML or XML). This language contains coding elements and is composed of these “cascading style sheets” which are equally called CSS files.***
## using the css
1. Inline - by using the style attribute inside HTML elements.
2. Internal - by using a <style> element in the <head> section.
3. External - by using a <link> element to link to an external CSS file.
## css selector 
<img src="https://cf.ppt-online.org/files/slide/k/Kbp3XcismqFREgGuz9OBIWY1vDx6MwHVeZQjC5/slide-8.jpg" width="250">

# introudction of Javascript
***JavaScript is a programming language commonly used in web development. It was originally developed by Netscape as a means to add dynamic and interactive elements to websites. This means JavaScript functions can run after a webpage has loaded without communicating with the server.***
## statments 
***Statements are used in JavaScript to control its program flow. Unlike properties, methods, and events, which are fundamentally tied to the object that owns them, statements are designed to work independently of any JavaScript object.***
#### Example :- 
var x, y, z;    // Statement 1
x = 5;          // Statement 2
y = 6;          // Statement 3
z = x + y;      // Statement 4
## comments 
You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code. 
#### Example :- 
/* Th i s script displays a greeting to the user based upon the current time.
It is an example from JavaScript & jQuer y book */
// Display the appropriate greeti ng based on the current time
## Variable
 ***means anything that can vary. JavaScript includes variables which hold the data value and it can be changed anytime. JavaScript uses reserved keyword var to declare a variable. A variable must have a unique name. ... In the above example, we have declared three variables using var keyword: one, two and three.***
**you define a variable in JavaScript**
***Declaring (Creating) JavaScript Variables Creating a variable in JavaScript is called "declaring" a variable. You declare a JavaScript variable with the var keyword: var carName; After the declaration, the variable has no value (technically it has the value of undefined ).***
## DATA TYPES 
1. NUMERIC DATA TYPE
The numeric data type handles
numbers.
5 
2. STRING DATA TYPE
The strings data type consists of
letters and other characters.
'hello there ' 
3. BOOLEAN DATA TYPE
Boolean data types can have one
of two values: true or false.
true 
## loops 
### USING LOGICAL OR , & , LOGICAL NOT
<img src="https://www.devopsschool.com/blog/wp-content/uploads/2020/07/JavaScript-Logical-Operator.png" width="250">

### Conditional Statements
1. Use if to specify a block of code to be executed, if a specified condition is true.
2. Use else to specify a block of code to be executed, if the same condition is false.
3. Use else if to specify a new condition to test, if the first condition is false.
#### Example :- 
if (time < 10) {
  greeting = "Good morning";
} else if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
