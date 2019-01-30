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
TML tags are element names surrounded by angle brackets:

<tagname>content goes here...</tagname>

- HTML tags normally come in pairs like ```<p>``` and ```</p>```
- The first tag in a pair is the start tag, the second tag is the end tag
- The end tag is written like the start tag, but with a forward slash inserted before the tag name

### The <!DOCTYPE> Declaration
- The <!DOCTYPE> declaration represents the document type, and helps browsers to display web pages correctly.
- It must only appear once, at the top of the page (before any HTML tags).
- The <!DOCTYPE> declaration is not case sensitive.

### HTML Documents
- All HTML documents must start with a document type declaration: <!DOCTYPE html>
- The HTML document itself begins with <html> and ends with </html>
- The visible part of the HTML document is between <body> and </body>

### HTML Headings
- HTML headings are defined with the <h1> to <h6> tags
- <h1> defines the most import heading. <h6> defines the least important hading
   
### HTML Paragraphs
- HTML paragraphs are defined with the <p> tag:


### HTML Links
<a>

```html
<a href="https://www.w3schools.com">This is a link</a>
```

- The link's destination is specified in the href attribute
- Attributes are used to provide additional information about HTML elements

### HTML Images
<img>

The source file (src), alternation text(alt), width, and height are provided as attributes

### HTML Buttons
<button>
   
### HTML Lists
- HTML lists are defined with the <ul>(unordered/bullet list) or the <ol> (ordered/numbered list) tag, followed by <li> tags(list times)
   
   
### Empty HTML Elements
- HTML elements with no content are called empty elements
- <br> is an empty element without a closing tag(<br> tag defins a line break)


## HTML Attributes

- All HTML elements can have attributes
- Attributes provide additional information about an element
- Attributes are always specified in the start tag
- Attributes usually come in name/value pairs like: ```html name = 'value'```
