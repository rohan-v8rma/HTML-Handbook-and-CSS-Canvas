# INDEX

- [HTML Reference](#html-reference)
    - [What is an HTML Element?](#what-is-an-html-element)
    - [Template of an HTML document](#template-of-an-html-document)
    - [What are HTML Attributes?](#what-are-html-attributes)
    - [What is the Role of a Web Browser in this process?](#what-is-the-role-of-a-web-browser-in-this-process)
    - [HTML Inline, Block & Flex elements](#html-inline-block--flex-elements)
        - [Block-level element](#block-level-element)
        - [Inline element](#inline-element)
        - [Inline-block](#inline-block)
            - [Features `display: inline-block` has over `display: inline`](#features-display-inline-block-has-over-display-inline)
            - [Features `display: inline-block` has over `display: block`](#features-display-inline-block-has-over-display-block)
        - [Flexbox](#flexbox)
    - [HTML elements](#html-elements)
        - [`<a>` element (Hyperlink tag)](#a-element-hyperlink-tag)
        - [`<img>` element](#img-element)
        - [`<div>` element](#div-element)
        - [`<header>` & `<footer>` element](#header--footer-element)
        - [`<link>` element](#link-element)
            - [Adding an external CSS stylesheet](#adding-an-external-css-stylesheet)
            - [Adding a favicon](#adding-a-favicon)

- [CSS Reference](#css-reference)
  - [What is CSS?](#what-is-css)
  - [Using CSS](#using-css)
  - [CSS Selectors](#css-selectors)
    - [CSS element Selector](#css-element-selector)
    - [CSS ID Selector](#css-id-selector)
    - [CSS class selector](#css-class-selector)
  - [CSS `display` Property](#css-display-property)
  - [CSS properties for flexboxes](#css-properties-for-flexboxes)
    - [`flex-direction` property](#flex-direction-property)
    - [`justify-content` property](#justify-content-property)
    - [`align-items` property](#align-items-property)
  - [CSS `text-decoration` property](#css-text-decoration-property)
    - [Removing the underline of a hyperlink](#removing-the-underline-of-a-hyperlink)

# HTML Reference

## What is an HTML Element?

An HTML element is defined by a start tag, some content, and an end tag:

```
<tagname> Content goes here... </tagname>
```
The HTML element is everything from the start tag to the end tag:
```
<h1>My First Heading</h1>
```
Some HTML elements have no content (like the `<br>` element). These elements are called **empty elements**. Empty elements do not have an end tag!

## Template of an HTML document

```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<p>My first paragraph.</p>

</body>
</html>
```

- `<!DOCTYPE html>` : This declaration defines that the document is an HTML5 document.<br> It is an instruction to the web browser about what version of HTML the page is written in. This ensures that the web page is parsed the same way by different web browsers. 
- `<html>` : This element is the root element of an HTML page and it defines the whole HTML document. 
- `<head>` : This element contains **meta information** (information about information) about the HTML page.
- `<title>` : This element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab).
- `<body>` : This element defines the document's body, and is a container for all the visible contents (which are displayed in a browser), such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
- `<p>` : This element defines a paragraph.

## What are HTML Attributes?

- HTML attributes provide additional information about HTML elements. All HTML elements can have attributes.
- Attributes are always specified in the start tag.
- Attributes usually come in name/value pairs like: `name="value"`

## What is the Role of a Web Browser in this process?

The purpose of a web browser (Chrome, Edge, Firefox, Safari) is to read HTML documents and display them correctly.

A browser does not display the HTML tags, rather it uses them to determine how to display the document.

## HTML Inline, Block & Flex elements

### Block-level element

A block-level element always starts on a new line, and the browsers automatically add some space (a margin) before and after the element. It always takes up the full width available (stretches out to the left and right as far as it can).

Two commonly used block elements are: `<p>` and `<div>`.

### Inline element

An inline element does not start on a new line. It only takes up as much width as necessary.

Some commonly used block elements are: `<img>`, `<a>` and `<span>`.

### Inline-block

An element with `display: inline-block` combines properties of inline and block.

#### Features `display: inline-block` has over `display: inline` 

- allows to set a width and height on the element.
- the top and bottom margins/paddings are respected.

#### Features `display: inline-block` has over `display: block` 

- does not add a line-break after the element, so the element can sit next to other elements.

### Flexbox

flex is a value which can be assigned to the CSS `display` property of an HTML element.

The Flexbox layout gives the container the ability to alter its items’ width/height (and order) to best fill the available space in order to accommodate to all kind of display devices and screen sizes. 

A flex container expands items to fill available free space or shrinks them to prevent overflow.

Most importantly, the flexbox layout is **direction-agnostic** as opposed to the regular layouts (block which is vertically-based and inline which is horizontally-based). 

While those work well for pages, they lack flexibility to support large or complex applications (especially when it comes to orientation changing, resizing, stretching, shrinking, etc.).

Refer 
[CSS properties for flexboxes](#css-properties-for-flexboxes) 
below or 
[A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) 
for more information.

## HTML elements

### `<a>` element (Hyperlink tag)

The HTML `<a>` element defines a hyperlink. It has the following attributes: 
- `href` : Contains the URL of the destination which the hyperlink leads to.
- `title` : Specifies extra information about an element. The information is shown as a **tooltip** text when the mouse moves over the element. 
- `target` :  Specifies where to open the linked document. By setting the target attribute to `"_blank"`, the linked document is opened in a new window or tab.

    Note that `target="_blank"` doesn't work in Markdown, meaning links from READMEs can't be opened in a new tab.

SYNTAX : 
```
<a href="url">Display text of hyperlink</a>
```
The hyperlink displays the text enclosed between the start and end tag to the user.

We can **remove the underline of a hyperlink** using [this](#removing-the-underline-of-a-hyperlink) method explained below.
<br> <br>

### `<img>` element

The HTML`<img>` element is used to embed an image in an HTML page.

Images are not technically inserted into a web page; images are linked to web pages. This element creates a holding space for the referenced image.
- `src` : Specifies the path to the image.
- `alt` : Specifies an alternate text for the image, if the image for some reason cannot be displayed. This text is also used by screen readers for telling about the image.
- `title` : Specifies the title of the image which is visible as a tooltip upon hovering on the image.
<br> <br>

### `<div>` element

The `<div>` tag is known as Division tag.

The Div is the most usable tag in web development because it helps us to separate out data in the web page and we can create a particular section for particular data or function in the web pages.

The `<div>` HTML element is a generic container for **flow content** (Flow content is a broad category that encompasses most elements that can go inside the `<body>` element, including heading elements, sectioning elements, etc). 

It has no effect on the content or layout until styled in some way using CSS.
<br> <br>

### `<header>` & `<footer>` element

`<header>` and `<footer>` are meta tags which just tell the browser that a header or a footer is being read. They behave like divs. It is recommended to use both of these tags to make our web page fully HTML5 compliant.
<br> <br>

### `<link>` element

The `<link>` element tells the relationship between the current document and an external resource.
It is most often used to link to external style sheets or to add a favicon  to a website.

It is an empty element, it contains attributes only which are as follows:
- `rel` : Specifies the relationship between the current document and the linked document.
- `href` : Specifies the location of the linked file.

#### **Adding an external CSS stylesheet**

```
<link rel="stylesheet" href="/css/styles.css">
```

#### **Adding a favicon**

```
<link rel="icon" href="/images/favicon.png">
```
NOTE: **favicon** is a small square image that represents a website in web browsers.

# CSS Reference

## What is CSS?


CSS (*Cascading Style Sheets*) is the language we use to style an HTML document. It is used to format the layout of a webpage, meaning how HTML elements should be displayed. <br>
NOTE: The word **cascading** refers to the fact that a style applied to a parent element will also apply to all children elements within the parent. <br>
So, if we set the color of the body text to "blue", all headings, paragraphs, and other text elements within the body will also get the same color (unless we specify something else).

## Using CSS

CSS can be added to HTML documents in 3 ways:

- **Inline** - Inline CSS uses the `style` attribute of an HTML element. This applies a unique style to a single HTML element.
```
...
<body>
    <h1 style = "color: limegreen;"> hello world </h1>    
</body>
...
```
- **Internal** - Internal CSS is used to define a style for a single HTML page. It is defined in the `<head>` section of an HTML page, within a `<style>` element.
```
...
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
...
```
- **External** - by using a `<link>` element to link to an external CSS file. We will be using the following attributes of the `<link>` HTML element:<br>
    - `rel` : Required. Specifies the relationship between the current document and the linked document
    - `href` : 	Specifies the location of the linked document, either as an absolute or relative URL.

```
...
<head>    
    <link rel="stylesheet" href="css/demostyles.css">
</head>
<body>
    <h1>hello world</h1>    
    <p>my name is rohan</p>
</body>
...
```

The most common way to add CSS, is to keep the styles in external CSS files. 

## CSS Selectors

Order of precedence for CSS:
ID > CLASS > ELEMENT
### CSS element Selector 

The element selector selects HTML elements based on the element name. <br>
Syntax:
```
<HTML-element> {
    color: red;
}
```

### CSS ID Selector 

The id selector uses the id attribute of an HTML element to select a specific element.

**The id of an element is unique within a page**, so the id selector is used to select one unique element. 
```
<p id = "para1">HelloWorld</p>
```

To select an element with a specific id, write a hash (#) character, followed by the id of the element. 
```
#para1 {
    color: red;
}
```
### CSS class selector

The class selector selects HTML elements with a specific class attribute. An element can be a part of multiple classes.
```
<p class = "firstclass secondclass">HelloWorld</p>
```

To select elements with a specific class, write a period `(.)` character, followed by the class name
```
.firstclass {
    color: red;
}
```

## CSS `display` Property

The `display` property specifies the display behavior (the type of rendering box) of an element.
Some common values for the display property are `inline`, `block`, `inline-block` and `flex`.

SYNTAX:
```
.class-name {
    display: display-property-value;
}
```

## CSS properties for flexboxes

SYNTAX:
```
.class-name {
    display: flex;
    flex-direction: row OR column;
    justify-content:
    align-items:
}
```

### `flex-direction` property

This establishes the main-axis, thus defining the direction flex items are placed in the flex container.

### `justify-content` property

This property defines the alignment along the **main-axis**. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size.

The possible values of this property are `flex-start`, `flex-end`, `space-around`, `space-between`, `space-evenly` and `center`.

### `align-items` property

This property defines the default behavior for how flex items are laid out along the cross axis on the current line. We can think of it as the justify-content version for the **cross-axis** (perpendicular to the main-axis).

## CSS `text-decoration` property 

### Removing the underline of a hyperlink

By setting the `text-decoration` of a certain class to none, the hyperlinks of that particular class will not be underlined, as links generally are by default. 
```
.class-name {
    text-decoration: none;
}
```
Be careful when removing the text decoration on anchors since users often depend on the underline to denote hyperlinks.

This is useful for removing hyperlink underlines from nav bars, a place where it's obvious a hyperlink is present and where we want to add our own formatting to the text.

