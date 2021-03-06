# HTML

HTML is the standard markup language for creating Web pages.

- HTML stands for Hyper Text Markup Language
- HTML describes the structure of Web pages using markup
- HTML elements are the building blocks of HTML pages
- HTML elements are represented by tags
- HTML tags label pieces of content such as "heading", "paragraph", "table", and so on
- Browsers do not display the HTML tags, but use them to render the content of the page

```html
<!DOCTYPE html>  <!--defines this document to be HTML5-->
<html> <!--is the root element of an HTML page-->
<head> <!--contains meta information about the document-->
<title>Page Title</title> <!--specifies a title for the document-->
</head>
<body> <!--contains the visible page content-->

<h1>My First Heading</h1>  <!--defines a large heading-->
<p>My first paragraph.</p>  <!--defines a paragraph-->

</body>
</html>
```

### HTML Tags
HTML tags are element names surrounded by angle brackets:

<tagname>content goes here...</tagname>

- HTML tags normally come in pairs like ```<p>``` and ```</p>```
- The first tag in a pair is the start tag, the second tag is the end tag
- The end tag is written like the start tag, but with a forward slash inserted before the tag name

### The <!DOCTYPE> Declaration
- The ```<!DOCTYPE>``` declaration represents the document type, and helps browsers to display web pages correctly.
- It must only appear once, at the top of the page (before any HTML tags).
- The ```<!DOCTYPE>``` declaration is not case sensitive.

### HTML Documents
- All HTML documents must start with a document type declaration: ```<!DOCTYPE html>```
- The HTML document itself begins with ```<html>``` and ends with ```</html>```
- The visible part of the HTML document is between ```<body>``` and ```</body>```

### HTML Headings
- HTML headings are defined with the ```<h1>``` to ```<h6>``` tags
- ```<h1>``` defines the most import heading. ```<h6>``` defines the least important hading
   
### HTML Paragraphs
- HTML paragraphs are defined with the ```<p>``` tag:


### HTML Links
```<a>```

```html
<a href="https://www.w3schools.com">This is a link</a>
```

- The link's destination is specified in the href attribute
- Attributes are used to provide additional information about HTML elements

### HTML Images
```<img>```

The source file (src), alternation text(alt), width, and height are provided as attributes

### HTML Buttons
```<button>```
   
### HTML Lists
- HTML lists are defined with the ```<ul>```(unordered/bullet list) or the ```<ol>``` (ordered/numbered list) tag, followed by ```<li>``` tags(list times)
   
   
### Empty HTML Elements
- HTML elements with no content are called empty elements
- ```<br>``` is an empty element without a closing tag(```<br>``` tag defins a line break)


## HTML Attributes

- All HTML elements can have attributes
- Attributes provide additional information about an element
- Attributes are always specified in the start tag
- Attributes usually come in name/value pairs like: ```html name = 'value'```

- ```href``` link address is specified in the ```href``` attribute
- ```src``` filename of the image source is specified in the ```src``` attribute
- ```width``` and ``` height``` specifies the width and the height of the image
- ```alt``` specifies an alternative text to be used, when an image cannot be displayed
- ```style``` specifies the styling of an element, like color, font, size etc
- ```lang``` declares the language of the document in the ```<html>``` tag
- ```title```  a ```title``` attribute is added to the ```<p>``` element. The value of the title attribute will be displayed as a tooltip when you mouse over the paragraph
- ```disabled``` specified that an input element should be disabled
- ```id``` specifies a unique id for an element


## HTML Headings
- Use HTML headings for headings only. Don't use headings to make text BIG or bold
- Search engines use the headings to index the structure and content of your web pages
- Users skim your pages by its headings. It's important to use headings to show the document structure
- Each HTML heading has a default size. However, you can specify the size for any heading with the ```style``` attribute, using the CSS ```font-size``` property

### HTML Horizontal Rules
- The ```<hr>``` tag defines a thematic break in an HTML page, and is most often displayed as a horizontal rule.
- The ```<hr>``` element is used to separate content (or define a change) in an HTML page

### The HTML ```<head>``` element
- The ```<head>``` element is a container for metadata. 
- HTML metadata is data about the HTML document
- Metadata is not displayed
- The ```<head>``` element is placed between the ```<html>``` tag and the ```<body>``` tag


## HTML Paragraphs

```<pre>``` element defines preformatted text

The text inside a ```<pre>``` element is displayed in a fixed-width font(usually Courier), and it preserves both spaces and line breaks 

### HTML Style Attribute

- Use the ```style``` attribute for styling HTML elements
- Use ```background-color``` for background color
- Use ```color``` for text colors
- Use ```font-family``` for text sizes
- Use ```text-align``` for text alignment


```html
<tagname style = "property:value;">
```
- The property is a CSS property
- The value is a CSS value


## HTML Formatting Elements

- ```<b>``` : Bold text
- ```<strong>``` : Important text
- ```<i>``` Italic text
- ```<em>``` Emphasized text
- ```<mark>``` Marked text
- ```<small>``` Small text
- ```<del>``` deleted text
- ```<ins>``` Inserted text
- ```<sub>``` Subscript text
- ```<sup>``` Superscript text

### HTML Quotation
- ```<q>```
   - Browser usually insert quotation marks around the ```<q>``` element

- ```<blockquote>```
   - Browsers usually indent <blockquote> elements
   
- ```<abbr>```
   - defines an abbreviation or an acronym. Marking abbreviations can give useful information to browsers, translation systems and search-engines.   

- ```<address>```
   - defines contact information(author/owner) of a document or an article
   - usually displayed in italic. Most browser will add a line break before and after the element
   
- ```<cite>```
   - defines the title of a work
   - usually display in italic

- ```<bdo>```
   - defines bi-directional override
   - override the current text direction

### HTML Comments

```html
<!-- This is a comment -->
```

## HTML Colors

- background color
```html
<h1 style="background-color:DodgerBlue;">Hello World</h1>
```
- text color
```html
<h1 style="color:Tomato;">Hello World</h1>
```
- border color
```html
<h1 style="border:2px solid Tomato;">Hello World</h1>
```

- [predefined color names](https://www.w3schools.com/colors/colors_names.asp)

- RGB Value: rgb(red, green, blue)
- HEX value: #rrggbb
- HSL Value: hsl(hue, saturation, lightness)
   - hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, 204 is blue
   - saturation is a percentage value, 0% means a shade of gray, 100% is the full color
   - llightness is also a percentage, 0% is black, 50% is neither light or dark, 100% is white
- RGBA value: rgba(red, green, blue, alpha)
   - alpha specifies the opacity for a color
- HSLA value: hsla(huem saturation, lightness, alpha)


## HTML Styles -CSS

- CSS stands for Cascading Style Sheets
- CSS describes how HTML elements are to be displayed on screen, paper, or in other media
- CSS saves a lot of work. It can control the layout of multiple web pages all at once
- CSS can be added to HTML elements in 3 ways:
   - Inline 
      - An inline CSS is used to apply a unique style to a single HTML element
      - An inline CSS uses the style attribute of an HTML element
   - Internal 
      - by using a ```<style>``` element in the ```<head>``` section
      - is used to define a style for a single HTML page
   - External 
      - by using an external CSS file
      - is used to define the style for many HTML pages
      - with an external style sheet, you can change the look of an entire website by changing one file
      - to use an external style sheet, add a link to it in the ```<head>``` section of the HTML page
         - full URL to link to a style sheet
         ```html
         <link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
         ```
         - style sheet located in the html folder on the current website
         ```html
         <link rel="stylesheet" href="/html/styles.css">
         ```
         - style sheet located in the same folder as the current page
         ```html
         <link rel="stylesheet" href="styles.css">
         ```
```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

```css
body {
  background-color: powderblue;
}
h1 {
  color: blue;
}
p {
  color: red;
}
```

```css
p {
  color: red; 
  font-family: courier;
  font-size: 160%;
  border: 1px solid powderblue;
  padding: 30px;
  margin: 50px;
}
```

### The id Attribute
- To define a specific style for one special element, add an id attribute to the element:
```html
<p id="p01"> I am different </p>
```
```css
#p01{
color:blue
}
```
### The class Attribute
- To define a style for special types of elements, add a class attribute to the element
```html
<p class="error"> I am different error</p>
```
```css
p.error{
color: yellow
}
```

## HTML Links
### Hyperlinks
- HTML links are hyperlinks
- You can click on a link and jump to another document
- When you move the mouse over a linke, the mouse arrow will turn into a little hand
- A link does not have to be text. It can be an image or any other HTML element

### Syntax
- In HTML, links are defined with the ```<a>``` tag

```html
<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>
```
### HTML Link Colors
Default link
- an unvisited linke is underlined and blue
- a visited link is underlined and purple
- an active link is underlined and red

You can change the default color by using CSS
```css
<!DOCTYPE html>
<html>
<head>
<style>
a:link {
  color: green;
  background-color: transparent;
  text-decoration: none;
}
a:visited {
  color: pink;
  background-color: transparent;
  text-decoration: none;
}
a:hover {
  color: red;
  background-color: transparent;
  text-decoration: underline;
}
a:active {
  color: yellow;
  background-color: transparent;
  text-decoration: underline;
}
</style>
</head>
<body>

<h2>Link Colors</h2>

<p>You can change the default colors of links</p>

<a href="html_images.asp" target="_blank">HTML Images</a> 

</body>
</html>
```

### The target Attribute
- The ```target``` attribute specifies where to open the linked document
- The ```target``` attribute can have one of the following values:
   - ```_blank```: opens the linked document in a new window or tab
   - ```_self```: opens the linked document in the same window/tab as it was clicked(default)
   - ```_parent```: opens the linked document in the parent frame
   - ```_top```: opens the linked document in the full body of the window 
   - ``` framename``` opens the linked document in a named frame
   

### Image as link

```html
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;">
</a>
```
### Link Titles
```html
<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
```

### Bookmark
- HTML bookmarks are used to allow readers to jump to specific parts of a web page
- bookmarks can be useful if your webpage is very long
- to make a book mark, you must first create the bookmark, and then add a link to it
- when the link is clicked, the page will scroll to the location with the bookmark

#### example
-First create a bookmark with the ```id``` attribute
```html
<h2 id="C4">Chapter 4</h2>
```
- Then, add a link to the bookmark('Jump to Chapter 4'), from within the same page:
```html
<a href="#C4">Jump to Chapter 4</a>
```
- Or, add a link to the bookmark from another page
```html
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```

### Image Maps
- the ```<map>``` tag defines an image-map
- An image-map is an image with clickable areas
- the ```name``` attribute of the ```<map>``` tag is associated with the ```<img>```'s usemap attribute and creates a relationship between the image and the map
- the ```<map>``` element contains a number of ```<area>``` tags, that define the clickable areas in the image map

### Background Image
- to add a background image on an HTML element, use the CSS property ```background-image```

### ```<picture>``` element
- the ```<picture>``` element contains a number of ```<source>``` elements, each referring to different image sources.
- The brower can choose the image that best fits the current view and/or device
- each ```<source>``` element have attributes describuing when their image is the most suitable
- the brower will use the first ```<source>``` element with matching attribute values, and ignore any following ```<source>``` elements

```html
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h2>The picture Element</h2>

<picture>
  <source media="(min-width: 650px)" srcset="img_pink_flowers.jpg">
  <source media="(min-width: 465px)" srcset="img_white_flower.jpg">
  <img src="img_orange_flowers.jpg" alt="Flowers" style="width:auto;">
</picture>

<p>Resize the browser to see different versions of the picture loading at different viewport sizes.
The browser looks for the first source element where the media query matches the user's current viewport width,
and fetches the image specified in the srcset attribute.</p>

<p>The img element is required as the last child tag of the picture declaration block.
The img element is used to provide backward compatibility for browsers that do not support the picture element, or if none of the source tags matched.
</p>

<p><strong>Note:</strong> The picture element is not supported in IE12 and earlier or Safari 9.0 and earlier.</p>

</body>
</html>
```

## HTML Table
- An HTML table is defined with the ```<table>``` tag
- each table row is defined with the ```<tr>``` tag
- A table header is defined with the ```<th>``` tag
- by default, table headings are bold and centered
- A table data/cell is defined with the ```<td>``` tag
- if you do not specify a border for the table, it will be dispalyed without borders
- a border is set using the CSS ```border``` property
```css
table, th, td {
  border: 1px solid black;
}
```
- if you want the boerders to collapse into one border, add the CSS border-collapse preperty
```css
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
```

## HTML Lists
- ```<ul>``` unordered list
- ``` list-style-type``` define list item marker: ```disc; circle; square; none```
- ```<ol>``` ordered list
- ```type``` numbering type: ```"1"; "A"; "a"; "I"; "i"```
- ```<li>``` define list item
- ```<dl>``` description list
- ```<dt>``` define description list
- ```<dd>``` describe the term in a description list
- list can be nested inside lists
- list items can contain other elements
- use css property ```float:left``` or ```display: inline``` to display a list horizontally


### Unordered List
```html
<ul style="list-style-type:disc;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

### Ordered list
```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
### Description Lists
```html
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```

### Horizontally navigation bar example

```html
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111111;
}
</style>
</head>
<body>

<h2>Navigation Menu</h2>
<p>In this example, we use CSS to style the list horizontally, to create a navigation menu:</p>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>

```

## HTML Block and inline Elements

### Block-level Elements
- a block level element always starts on a new line and takes up the full width available
```<address><article><aside><blockquote><canvas><dd><div><dl><dt><fieldset><figcaption><figure?<footer><form><h1>-<h6><header><hr><li><main><nav><noscript><ol><output><p><pre><section><table><tfoot><ul><video>```

### Inline Elements
- an inline element does not start on a new line and only takes up as much width as necessary
```<a><abbr><acronym><b><bdo><big><br><button><cite><code><dfn><em><i><img><input><kbd><label><map><object><q><samp><script><select><small><span><strong><sub><sup><textarea><time><tt><var>```

- ```<div>``` used as a container for other HTML elements
- ```<div>``` no required attributes, but ```style```, ```class```, ```id``` are common
- when used together with CSS, the ```<div>``` element can be used to sytle blocks of content
- ```<span>``` used as a container for some text
- ```<span>``` no required attributes, but ```style```, ```class```, ```id``` are common
- when used together with CSS, the ```<span>``` element can be used to style parts on the text

## class Attribute
- class attribute is used to define equal styles for elements with the same class name
- the class attribute can be used on any HTML element
- the class name is case sensitive
- HTML elements can have more than one class name, each class name must be seperated by a space
- different tags can have the same class name and thereby share the same style

## id Attribute
- the id attribute specifies a unique id for an HTML element
- in CSS, to select an element with a specific id, write a hash(#) character, followed by the id of the element
- the id attribute can be used on any HTML element
- the id value is case-sensitive
- the id value must contain at least one character, and must not contain whitespace
- an HTML element can only have one unique id that belongs to that single element, while a class name can be used by multiple elements

## Iframes
- an HTML iframe is defined with the ```<iframe>``` tag

```html
<iframe src="URL" ></iframe>
```

- an iframe can be used as the target frame for a link
- the ```target``` attribute of the link must refer to the ```name``` attribute of the iframe

```html
<iframe src = "demo_iframe.htm" name="iframe_a"></iframe>

<p><a href="http://khrfewia.com" target = "iframe_a"> aietjeaw</a></p>
```

## HTML JavaScript
### ```<script>``` 
- ```<script>``` tag is used to define a client side script(JavaScript).
- ```<script>``` element either contains scripting statements, or it points to an external script file through the ```src``` attribute
- ```<noscript>``` defines an alternate content for users that do not support client-side scripts

### change HTML Content
```html
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript"
</script>
```

### change HTML style
```html
<script>
document.getElementById("demo").style.fontSize = "50px"
</script>
```
### change HTML attributes
```html
<script>
document.getElementById("demo").src = "picture.gif"
</script>
```

## HTML file paths
- a file path describes the location of a file in a web site's folder structure
- file paths are used when linking to external files like:
   - web pages
   - images
   - style sheets
   - javascripts
   
### Absolute File Paths
- an absolute file path is the full URL to an internet file

### Relative File Paths
- a relative file path points to a file relative to the current page

### Best Practice
- it is best practice to use relative file paths
- when using relative file paths, your web pages will not be bound to your current base URL. All links will work on your own computer as well as on your current public domain and your future public domains



## HTML Head

- ```<head>``` element is a container for metadata(data about data) and is placed between the ```<html>``` tag and the ```<body>``` tag
- HTML metadata is not displayed
- metadata typically define the document title, character set, styles, links, scripts, and other meta information

### ```<title>```
- ```<title>``` element defines the title of the document, and is required in all HTML
- defines a title in the brower tab
- provides a title for the page when it is added to favorites
- displayed a title for the page in search engine results


### ```<style>```
- the ```<style>``` element is used to define style information for a single HTML page

### ```<link>```
- ```<link> element used to link to external style sheets

```html
<link rel="stylesheet" href="mystyle.css">
```

### ```<meta>```
- the ```<meta>``` element is used to specify which character set is used, page description, keyowrd, author, and otehr metadata
- metadata is used by browsers(how to display content), by search engines(keywords), and other web services

```html
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="keywords" content="HTML, CSS, XML, JavaScript">
<meta name="author" content="John Doe">
<meta http-equiv="refresh" content="30">
```

### Viewport
- the viewport is the user's visible area of a web page. It varies with the device, and will be smaller on a mobile phone than on a computer screen
- you should include the follow ```<meta>``` viewport element  in all your web pages:
```html
<meta name = "viewport" content = "width=device-width, initial-scale=1.0">
```
- a ```<meta>``` viewport element gives the browser instructions on how to control the page's dimensions and scaling
- The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

- The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.

### ```<base>```

- the ```<base>``` element specifies the base URL and base target for all relative URLs in a page
```html
<base href="https://www.w3schools.com/images/" target="_blank">
```

## Computer code elements
### ```<kbd>```
- ```<kbd>``` element represents user input, like keyboard input to voice commands
- text surrounded by ```<kbd>``` tags is typically displayed in the browser's default monospace font
### ```<samp>```
- the ```<samp>``` element represent output from a program or computing system
- text surround by ```<samp>``` tags is typically displayed in the browser's default monospace font

### ```<code>```
- ```<code>``` element defines a fragment of computer code
- text surrounded by ```<code>``` tags is typically displayed in the browser's default monospace font
- ```<code>``` element does not preserve extra whitespace and line-breaks

### ```<var>```
- ```<var>``` element defines a variable
- the variable could be a variable in a mathematical expression or a variable in programming context


## HTML Form
### ```<form>```
- the HTML ```<form>``` element defines a form that is used to collect user input:
- an HTML form contains form elements
- form elements are different types of input elements, like text fields, check boxed, radio buttons, submit buttons, and more

### ```<input>```
- the ```<input>``` element can be displayed in serveral ways, depending on the type attribute
| Type | Desciption |
| --- | ---:|
| ```<input type="text">``` | defines a one-line text input field |
| ```<input type="radio">``` | defines a radio button(for selecting one of many choices) |
| ```<input type="submit">``` | defines a submit button(for submitting the form) |

#### the submit button
- ```<input type="submit">``` defines a button for submitting the form data to a form-handler.
- The form-handler is typically a server page with a script for processing input data.
- The form-handler is specified in the form's action attribute:

```html
<form action="/action_page.php">
  First name:<br>
  <input type="text" name="firstname" value="Mickey"><br>
  Last name:<br>
  <input type="text" name="lastname" value="Mouse"><br><br>
  <input type="submit" value="Submit">
</form>
```
### The Action Attribute
- the ```action``` attribute defines the action to be performed when the form is submitted
- normally, the form data is sent to a web page on the server when the user clicks on the submit button
- if the ```action``` attribute is omitted, the action is set to the current page

### The Target Attribute
- the target attribute specifies if the submitted result will open in a new browser tab, a frame, or in the current window
- the default value is "```_self```" which means the form will be submitted in the current window
- to make the form result open in a new browser tab, use the value "```_blank```"

### The Method Attribute
- The method attribute specidies the HTTP method(GET or POST) to be used when submitting the form data

#### GET
- the default method when submitting form data is GET
- When GET is used, the submitted form data will be visible in the page address field
- appends form-data into the URL in name/value pairs
- the length of a URL is limited
- never use GET to send sensitive dta
- useful for form submissions where a user wants to bookmark the result
- GET is better for non-secure data, like query strings in Google

#### POST
- always use POST if the form data contains sensitive or personal information
- the POST method does not display the submitted form data in the page address field
- POST has no size limitations, and can be used to send large amounts of data
- form submissions with POST cannot be bookmarked

### The Name Attribute
- each input field must have a name attribute to be submitted 
- if the name attribute is omitted, the data of that input field will not be sent at all

### Grouping Form Data with ```<fieldset>```
- the ```<fieldset>``` element is used to group related data in a form
- the ```<legend>``` element defines a caption for the ```<fieldset>``` element

## HTML Form Elements

### ```<input>```
### ```<select>```
- defines a drop-down list:
- ```<option>``` elements define an option that can be selected
- By default, the first item in the drop-down list is selected.
- To define a pre-selected option, add the selected attribute to the option:
- use the size attribute to specify the number of visible values
- use the multiple attribute to allow multiple selections

```html
<select name="cars" size="3" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat" selected>Fiat</option>
  <option value="audi">Audi</option>
</select>
```

### ```<textarea>```
- defines a multi-line input field
- the rows attribute specifies the visible number of lines in a text area
- the cols attribute specifies the visible width of a text area
- you can also define the size of the text area by using CSS style

```html
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
```

### ```<button>```
- defines a clickable button






