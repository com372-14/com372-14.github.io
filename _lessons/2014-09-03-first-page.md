---
layout: post
title: Making your first page
lesson_num: '04'
class_date: September 3, 2014
lead: Now that we are familiar with the basic structure and syntax of HTML, let's write our first page!
---

## Due For This Class

_Both items are due at the start of class_

- Read [A Brief History of Markup](http://alistapart.com/article/a-brief-history-of-markup)
- Complete first lesson in the CodeCademy [Web Fundamentals](http://www.codecademy.com/tracks/web) track.  Email me the screenshot of your completed lesson.

<!--## Presentation

<iframe src="https://docs.google.com/presentation/embed?id=1_CGlKMEB6eVm5em64rxw1eoiiZHxjkbRlaVXRwyIolw&amp;start=false&amp;loop=false&amp; frameborder="0" width="520" height="405"></iframe>
-->

## More Common HTML Terms
  
### Attributes

The tag may contain additional information and such information is called an attribute. Tags such as `<img>` and `<a>` use attributes. Attributes usually consist of 2 parts:

- An attribute name (such as `src` or `href`)
- An attribute value (such as `doge.jpg` or `link.html`)
- Attribute values should be wrapped in quote marks (" or ').  I recommend using double-quotes.  Whatever you choose, stay consistent.

```html
<img src="myimage.jpg" alt="A great selfie!">
```

```html
<img src='myimage.jpg' alt='SJU Campus'>
```

**Important note about using quote marks** - When you are working with quote marks, you will need to be careful of using quotes within your attributes.  When possible, use the opposite type of quote mark than what you will write within the value.

```html
<img src="myimage.jpg" alt="Saint Joseph's Campus">
```

```html
<img src='myimage.jpg' alt='The dog said "Woof!"'>
```

Or you can use encoded characters.

```html
<img src="myimage.jpg" alt="Some &quot;text&quot;">
```

## Coding Standards

The way that you write code matters from a readability standpoint. While your code may work and validate if you do not follow these guidelines, it is important that you learn to write code neatly and cleanly.

Here are some basic guidelines.  We will expand these as you progress through this course.

1) Use all lowercase in tag names (with the exception of DOCTYPE - you can choose what you would like to do for this)

*Good*
```html
<p>This is my <strong>important</strong> text.</p>
```
*Bad*
```html
<P>This is my <STRONG>important</STRONG> text.</P>
```

2) Start the following tags on new lines

```html
<p>, <div>, <h1> - <h6>, <ul>, <li>
```

There are more tags that it would make sense for starting on new lines, but we have not learned them yet.

3) Don't start the following tags on new lines (unless doing so helps with the readability of your code - can especially be the case when, for example, you're wrapping an image in an anchor)

```html
<strong>, <em>, <a>, <img>
```

4) Indent with two spaces (your IDE should help you do this - when we start using an IDE I will discuss with you how to set this up).

If you're interested, there are many style guides out there.  

- [Google](https://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml)
- [MDO](http://codeguide.co/)
- [Paul Robert Lloyd](http://paulrobertlloyd.com/about/styleguide/) - this addresses reasoning for using specific elements

And just for fun, here is TimBL's [original style guide](http://www.w3.org/Provider/Style/)

5) Use a reasonable amount of empty lines to separate your code if you think it helps with readabilty.  Not all tags need to be separated by full empty lines. Don't use extraneous whitespace - use 1 empty line rather than 5.

6) Use comments as much as you want in the beginning!  Comments are great, particularly for you to mark where you may be having difficulties with your code or to justify your coding choices.


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

### Project 1 - Using HTML to Structure Text (due 9/3/2014)

1. Complete Project 1.  The instructions are in the project page.
2. As the course moves on, we will add project information to our *Project Portfolio*.  This is your first entry into your Project Portfolio.  Bring your completed project to class on Wednesday, and we will walk through adding it to your Project Portfolio using Github.