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

# CSS Reference

CSS (*Cascading Style Sheets*) is the language we use to style an HTML document. It is used to format the layout of a webpage, meaning how HTML elements should be displayed. <br>
NOTE: The word **cascading** refers to the fact that a style applied to a parent element will also apply to all children elements within the parent. <br>
So, if we set the color of the body text to "blue", all headings, paragraphs, and other text elements within the body will also get the same color (unless we specify something else).

