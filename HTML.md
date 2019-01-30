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

- ![predefined color names](https://www.w3schools.com/colors/colors_names.asp)



















