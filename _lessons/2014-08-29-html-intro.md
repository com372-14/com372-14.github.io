---
layout: post
title: Introduction to HTML
lesson_num: '03'
class_date: August 29, 2014
lead: Hypertext Markup Language (HTML) is the basis of every page on the web. HTML provides the meaning and structure to our pages.
---

## Due Today

- Read Chapters 1 and 2 of the Robbins book.

## Presentation

<iframe src="https://docs.google.com/presentation/embed?id=1_CGlKMEB6eVm5em64rxw1eoiiZHxjkbRlaVXRwyIolw&amp;start=false&amp;loop=false&amp; frameborder="0" width="520" height="405"></iframe>

## What is HTML?

HTML is a markup language. It tells the web browser what content to display. HTML separates "content" (words, images, audio, video, and so on) from "presentation" (the definition of the type of content and the instructions for how that type of content should be displayed). HTML uses a pre-defined set of elements to identify content types. Elements contain one or more "tags" that contain or express content. Tags are surrounded by angle brackets, and the "closing" tag (the one that indicates the end of the content) is prefixed by a forward slash.

For example, the paragraph element consists of the start tag `<p>` and the closing tag `</p>`. The following example shows a paragraph contained within the HTML paragraph element:

```html
<p>You are beginning to learn HTML.</p>
```

When this content is displayed in a web browser, it looks like this:

You are beginning to learn HTML.

The browser uses the tags as an indicator of how to display the content in the tags.

Elements that contain content can usually also contain other elements. For example, the emphasis element (`<em>`) can be embedded within a paragraph element, to add emphasis to a word or phrase:

```html
<p>You are <em>beginning</em> to learn HTML.</p>
```

When displayed, this looks like:

You are *beginning* to learn HTML.

Some elements do not contain other elements. For example, the image tag ("<img>") specifies the file name of the content (an image) as an attribute:

```html
<img src="smileyface.jpg">
```

"What is HTML" is from Mozilla Developer Networks' [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Introduction)

## Common HTML terms

### Elements 

Elements define the semantic meaning of their content. Elements include everything between two matching element tags, including the tags themselves. For example, the ```<p>``` element indicates a paragraph; the ```<img>``` element indicates an image.

The following is a paragraph element:

```html
<p>
This is the content of the paragraph element.
</p>
```

### Tags 

Tags are used to mark up the start and end of an HTML element.

  A start tag consists of an opening angle bracket (<) followed by the element name, zero or more space separated attribute/value pairs, and a closing angle bracket (>).
  
  A start tag with no attributes:
  
  ```html
  <p>
  ```
  
  A start tag with an attribute:
  
  ```html
  <p class="info">
  ```
  
  End tags consist of an opening angle bracket followed by a forward slash, the element name, and a closing angle bracket:
  
  ```html
  </p>
  ```
  
  **Void elements** are empty, meaning that they only consist of a single tag and do not have any content. In HTML, such tags look just like opening tags:
  
  ```html
  <br>
  ```
  
  Void elements (tags that do not need to be closed) can also contain attributes.
  
  ```html
  <img src="smile.jpg">
  ```

  Depending on what type of HTML you are writing, you may find that your code will not validate without properly closing all tags, including void tags.  This is typically the case if you are writing XHTML.  The appropriate way to close a void tag is to add a closing slash before the end of the tag.
  
  ```html
  <img src="smile.jpg" />
  ```
  
  **Extra reading** [To Close or Not to Close](http://www.colorglare.com/2014/02/03/to-close-or-not-to-close.html)
  
  In this course, I will not deduct points if you choose to close your void tags (using the appropriate syntax, as demonstarted above).  Please just be consistent.
  
  
### Attributes

The tag may contain additional information and such information is called an attribute. Tags such as `<img>` and `<a>` use attributes. Attributes usually consist of 2 parts:

- An attribute name (such as `src` or `href`)
- An attribute value (such as `doge.jpg` or `link.html`)

### Doctype
In addition to tags, text content, and entities, an HTML document must contain a doctype declaration as the first line. The doctype declaration is not an HTML tag; it is an instruction to the web browser about what version of HTML the page is written in.

Adapted from Mozilla Developer Networks' [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Introduction)


HTML documents are written in plain text. They can be written in any text editor that allows content to be saved as plain text, such as Notepad, Notepad++, or Sublime,  but most HTML authors prefer to use a specialized editor that highlights syntax and shows the DOM. 

## Common HTML Tags

```html
<p>This is a paragraph</p>

<h1>Heading Level 1</h1>
<h2>Heading Level 2</h2>
<h3>Heading Level 3</h3>
<h4>Heading Level 4</h4>
<h5>Heading Level 5</h5>
<h6>Heading Level 6</h6>

<em>Emphasis, aka italics</em>
<strong>Strong, aka bold</strong>

<ul>
    <li>Unordered list item 1</li>
    <li>Unordered list item 2</li>
    <li>Unordered list item 3</li>
</ul>

<ol>
    <li>Ordered list item 1</li>
    <li>Ordered list item 2</li>
    <li>Ordered list item 3</li>
</ol>

<a href="http://www.google.com/">This is a link</a>

<img src="pizza.jpg">

<!-- This is a comment. Anything put here will not appear on the page -->
```

For a full list of HTML tags, check out the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

## Starter HTML Template

A very basic HTML page:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>PAGE TITLE</title> <!-- DON'T FORGET THE TITLE -->
  </head>
  <body>
  <!-- PLACE ALL OF YOUR PAGE CONTENT BELOW HERE -->

  <h1>This is my heading</h1>

  <p>This is a paragraph</p> 

  <!-- AND ABOVE HERE -->
  </body>
</html>
```

**[Our starter HTML template is available to download on Github](https://github.com/com372-14/page-template).**


## Homework

### Read

[A Brief History of Markup](http://alistapart.com/article/a-brief-history-of-markup)

### Codeacademy (due 9/3/2014)
1. Sign up for an account at [codeacademy.com](http://www.codecademy.com/).
2. Select the [Web Fundamentals](http://www.codecademy.com/tracks/web) track.
3. Complete lesson 1 HTML Basics (**note: there are 13 steps to this lesson**).
4. To verify you have completed this lesson [take a screenshot](http://www.take-a-screenshot.org/) of  page that clearly shows you have completed the lesson and email it to me ([kpipe@sju.edu](mailto:kpipe@sju.edu)).