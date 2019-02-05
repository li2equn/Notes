# CSS-learning

## CSS Syntax and Selectors

### CSS Syntax

A CSS rule-set consist of a selector and a devlaration block

The selector points to the HTML element you want to style.

The declaration block contains one or more declarations separated by semicolons.

Each declaration includes a CSS property name and a value, separated by a colon.

A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces.

```css
p {
  color: red;
  text-align: center;
}
```

### CSS Selectors
CSS selectors are used to "find" (or select) HTML elements based on their element name, id, class, attribute, and more.

#### The element Selector
The element selector selects elements based on the element name.

You can select all <p> elements on a page like this (in this case, all <p> elements will be center-aligned, with a red text color):
  
  ```css
  p {
  text-align: center;
  color: red;
}
  ```

#### The id Selector

The id selector uses the id attribute of an HTML element to select a specific element.

The id of an element should be unique within a page, so the id selector is used to select one unique element!

To select an element with a specific id, write a hash (#) character, followed by the id of the element.

The style rule below will be applied to the HTML element with id="para1":

```css
#para1 {
  text-align: center;
  color: red;
}
```

#### The class Selector

The class selector selects elements with a specific class attribute.

To select elements with a specific class, write a period (.) character, followed by the name of the class.

In the example below, all HTML elements with class="center" will be red and center-aligned:

```css
.center{
text-align:center;
color:red;
}
```

#### CSS Comments
A CSS comment starts with ```/*``` and ends with ```*/```

```css
p {
  color: red;
  /* This is a single-line comment */
  text-align: center;
}

/* This is
a multi-line
comment */
```

## CSS How To
### External Style Sheet

Each page must include a reference to the external style sheet file inside the <link> element. The <link> element goes inside the <head> section:
```html
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```
An external style sheet can be written in any text editor. The file should not contain any html tags. The style sheet file must be saved with a .css extension.

Here is how the "mystyle.css" looks:

```css
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```

### Internal Style Sheet
Internal styles are defined within the <style> element, inside the <head> section of an HTML page:

```html
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
} 
</style>
</head>
```

### Inline Style

An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

The example below shows how to change the color and the left margin of a <h1> element:

```html
<h1 style="color:blue;margin-left:30px;">This is a heading</h1>
```

### Oascading Order

1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default









