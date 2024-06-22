# HTML Notes

## Introduction to HTML
HTML (HyperText Markup Language) is the standard language for creating web pages and web applications. It describes the structure of a webpage using markup.

## Basic Structure of an HTML Document
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <h1>Hello, World!</h1>
</body>
</html>

HTML Elements
HTML elements are the building blocks of HTML pages.

Headings
HTML

<h1>This is a heading</h1>
<h2>This is a subheading</h2>
AI-generated code. Review and use carefully. More info on FAQ.
Paragraphs
HTML

<p>This is a paragraph.</p>
AI-generated code. Review and use carefully. More info on FAQ.
Links
HTML

<a href="https://www.example.com">This is a link</a>
AI-generated code. Review and use carefully. More info on FAQ.
Images
HTML

<img src="image.jpg" alt="Description of image">
AI-generated code. Review and use carefully. More info on FAQ.
Lists
Ordered List

HTML

<ol>
  <li>First item</li>
  <li>Second item</li>
</ol>
AI-generated code. Review and use carefully. More info on FAQ.
Unordered List

HTML

<ul>
  <li>First item</li>
  <li>Second item</li>
</ul>
AI-generated code. Review and use carefully. More info on FAQ.
Tables
HTML

<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>
AI-generated code. Review and use carefully. More info on FAQ.
Forms
HTML

<form action="/submit" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <input type="submit" value="Submit">
</form>
AI-generated code. Review and use carefully. More info on FAQ.
Buttons
HTML

<button type="button">Click Me!</button>
AI-generated code. Review and use carefully. More info on FAQ.
Div and Span
HTML

<div>
  <p>This is a block-level element.</p>
</div>

<span>This is an inline element.</span>
AI-generated code. Review and use carefully. More info on FAQ.
Semantic Elements
HTML

<header>
  <h1>Header</h1>
</header>
<nav>
  <a href="#home">Home</a>
  <a href="#about">About</a>
</nav>
<main>
  <article>
    <h2>Main Content</h2>
    <p>This is the main content of the page.</p>
  </article>
</main>
<footer>
  <p>Footer</p>
</footer>
AI-generated code. Review and use carefully. More info on FAQ.
Attributes
HTML attributes provide additional information about elements.

Global Attributes
class: Specifies one or more class names for an element
HTML

<div class="container"></div>
AI-generated code. Review and use carefully. More info on FAQ.
id: Specifies a unique id for an element
HTML

<p id="uniqueParagraph"></p>
AI-generated code. Review and use carefully. More info on FAQ.
style: Specifies inline CSS styles
HTML

<p style="color: red;">This is a red paragraph.</p>
AI-generated code. Review and use carefully. More info on FAQ.
title: Provides additional information about an element (displayed as a tooltip)
HTML

<p title="This is a tooltip">Hover over me</p>
AI-generated code. Review and use carefully. More info on FAQ.
HTML Comments
Comments are used to insert notes in the HTML code. They are not displayed in the browser.

HTML

<!-- This is a comment -->
<p>This is a paragraph.</p>
AI-generated code. Review and use carefully. More info on FAQ.
HTML Entities
HTML entities are used to display reserved characters.

HTML

<p>Tom & Jerry</p> <!-- Displays "Tom & Jerry" -->
<p>5 &lt; 10</p> <!-- Displays "5 < 10" -->
AI-generated code. Review and use carefully. More info on FAQ.
Doctype
The <!DOCTYPE> declaration represents the document type and helps browsers to display web pages correctly. It must be the very first thing in your HTML document, before the <html> tag.

HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Document</title>
</head>
<body>
</body>
</html>
AI-generated code. Review and use carefully. More info on FAQ.
Character Encoding
Setting the character encoding is important for the proper display of text content. UTF-8 is the most widely used character encoding.

HTML

<meta charset="UTF-8">
AI-generated code. Review and use carefully. More info on FAQ.
Viewport
The viewport meta tag helps with responsive web design.

HTML

<meta name="viewport" content="width=device-width, initial-scale=1.0">
AI-generated code. Review and use carefully. More info on FAQ.
Linking CSS and JavaScript
Linking an External CSS File

HTML

<link rel="stylesheet" href="styles.css">


11. HTML5 New Elements
HTML5 introduced several new elements to improve the structure of HTML documents:

<header>: Defines a header for a document or section.
<nav>: Defines a set of navigation links.
<section>: Defines a section in a document.
<article>: Defines an independent, self-contained content.
<aside>: Defines content aside from the main content (like a sidebar).
<footer>: Defines a footer for a document or section.
<figure>: Specifies self-contained content, such as illustrations, diagrams, photos, code listings, etc.
<figcaption>: Defines a caption for a <figure> element.
Example usage:

HTML

<article>
  <header>
    <h1>Article Title</h1>
    <p>Author: John Doe</p>
  </header>
  <section>
    <h2>Section Title</h2>
    <p>This is a section within the article.</p>
  </section>
  <footer>
    <p>Published on: January 1, 2021</p>
  </footer>
</article>
AI-generated code. Review and use carefully. More info on FAQ.
12. HTML5 Input Types
HTML5 introduced new input types for better forms:

email: Validates the input as an email address.
HTML

<input type="email">
AI-generated code. Review and use carefully. More info on FAQ.
tel: Validates the input as a telephone number.
HTML

<input type="tel">
AI-generated code. Review and use carefully. More info on FAQ.
url: Validates the input as a URL.
HTML

<input type="url">
AI-generated code. Review and use carefully. More info on FAQ.
number: Allows input of numeric values.
HTML

<input type="number">
AI-generated code. Review and use carefully. More info on FAQ.
range: Allows input of a number within a specified range.
HTML

<input type="range" min="1" max="10">
AI-generated code. Review and use carefully. More info on FAQ.
date: Allows input of a date.
HTML

<input type="date">
