# HTML 
## images
### Adding Images


* The HTML < img> tag is used to embed an image in a web page.

* Images are not technically inserted into a web page; images are linked to web pages. The < img> tag creates a holding space for the referenced image.

*The < img> tag is empty, it contains attributes only, and does not have a closing tag.

* The < img> tag has two required attributes:

1. src - Specifies the path to the image.
2. alt - Specifies an alternate text for the image.


### The src Attribute

* The required src attribute specifies the path (URL) to the image.

> Note: When a web page loads; it is the browser, at that moment, that gets the image from a web server and inserts it into the page. Therefore, make sure that the image actually stays in the same spot in relation to the web page, otherwise your visitors will get a broken link icon. The broken link icon and the alt text are shown if the browser cannot find the image.The HTML < a> tag defines a hyperlink. It has the following syntax:

> < img src="img_chania.jpg" alt="Flowers in Chania">




### The alt Attribute

* The required alt attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).

The value of the alt attribute should describe the image:



> < img src="img_chania.jpg" alt="Flowers in Chania">


### Width and Height, or Style?


* The width, height, and style attributes are all valid in HTML.

* However, we suggest using the style attribute. It prevents styles sheets from changing the size of images:

### Images in Another Folder
* If you have your images in a sub-folder, you must include the folder name in the src attribute:
> < img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;"

### Images on Another Server/Website

* Some web sites point to an image on another server.

* To point to an image on another server, you must specify an absolute (full) URL in the src attribute:
> < img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">

### Animated Images
* < img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">
### Image as a Link

* To use an image as a link, put the < img> tag inside the < a> tag:


> < a  href="default.asp">
  < img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
< /a>
### Image Floating
* Use the CSS float property to let the image float to the right or to the left of a text:

> < p>< img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image will float to the right of the text.</ p>

> < p>< img src="smiley.gif" alt="Smiley fac8e" style="float:left;width:42px;height:42px;">
The image will float to the left of the text.</ p>

### Common Image Formats


Abbreviation	File Format	File Extension
APNG	Animated Portable Network Graphics	.apng
GIF	Graphics Interchange Format	.gif
ICO	Microsoft Icon	.ico, .cur
JPEG	Joint Photographic Expert Group image	.jpg, .jpeg, .jfif, .pjpeg, .pjp
PNG	Portable Network Graphics	.png
SVG	Scalable Vector Graphics	.svg

<img src=https://blog.filestack.com/wp-content/uploads/2019/03/image-file-extensions.png alt=common images>

### Chapter Summary

* Use the HTML < img> element to define an image
* Use the HTML src attribute to define the URL of the image
* Use the HTML alt attribute to define an alternate text for an image, if it cannot be displayed
* Use the HTML width and height attributes or the CSS width and height properties to define the size of the image
* Use the CSS float property to let the image float to the left or to the right.

>  Loading large images takes time, and can slow down your web page. Use images carefully.


## color
> this photo explain what is the type of color :-
<img src=https://www.webfx.com/blog/images/assets/cdn.sixrevisions.com/0138-02_color_methods.png alt=common >


## font 
### Specifying Typefaces
#### font-family
* The font-family property allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.



### Navigation Bar

#### font-size

* The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font.

### Bold
#### font-weight

* The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:
1. normal

**This causes text to appear at a normal weight.**
2. bold
**This causes text to appear bold.**

* column (often used for mobile browsers)
* column (often used for tablets and laptops)
* column layout (only used for desktops)


### Italic
#### font-style

* If you want to create italic text,
you can use the font-style
property. There are three values
this property can take:
1. normal

**This causes text to appear in a normal style (as opposed to italic or oblique).**
2. italic
**This causes text to appear italic.**
3. oblique
**This causes text to appear oblique** 

### uppercase and lowercase
#### text-transform
* The text-transform property
is used to change the case of
text giving it one of the following
values:

1. uppercase
**This causes the text to appear uppercase.**
2. lowercase
**This causes the text to appear lowercase.**
3. capitalize
**This causes the first letter of each word to appear capitalized.**

### Underline & Strike
#### text-decoration
* The text-decoration property
allows you to specify the
following values:

1. none
**This removes any decoration already applied to the text.**
2. overline
**This adds a line over the top of the text.**
3. line-through
**This adds a line through words.**

4. blink
**This animates the text to make it flash on and off (however this is generally frowned upon, as it is considered rather annoying)**

> ant other things for TEXT we can find it in html and css books . 


### TL;DR
* Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.