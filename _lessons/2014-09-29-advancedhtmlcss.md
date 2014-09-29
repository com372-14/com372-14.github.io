---
layout: post
title: Advanced HTML & CSS
lesson_num: '15'
week_num: 6
class_date: September 29, 2014
lead: 
dontlink: false
---

## Due For This Class

- Start working on Project #4.  It will be due next Friday (October 3, 2014)
- Finish coding your resume.  Upload to GitHub.

## Lesson

1. Combining Selectors
2. Spacing within selectors
3. Layering styles (btn, btn + btn-danger)
4. Centering things with CSS

## CSS Selectors - Review

A CSS selector is the part of the rule set that defines the content that you are styling.  There are many different kinds of selectors.

### Element Selector

We have mostly been using element selectors in class so far.  In order to apply to the page, the selector must match one or more element that you’re using in your page.  A selector of `p` would match all of the `<p>` you’re using, while a selector of `li` would match all of your list items.

Let’s look at some sample CSS.

```css
ul{
	list-style:none;
	border: 4px solid red;
	color: blue;
}
```

And here is some HTML that we might apply this CSS to.

```html
<ul>
  <li>Fish</li>
  <li>Apples</li>
  <li>Cheese</li>
</ul>

<div class="example">
  <p>Example paragraph text.</p>
</div>

<ul>
  <li>Water</li>
  <li>Juice</li>
  <li>Maple Syrup</li>
</ul>
```

The `ul` selector matches *both* of the `<ul>` elements on this page.  If we changed the selector to `div`, the styles would be applied to the `<div>` element instead.

Styles are not automatically applied to child elements of the selected element, but some styles may be inherited.  In this example, the `color` rule would be inherited (all children of the selector would have the same color as set in the selector, unless set differently elsewhere).


### ID Selector

In CSS, you write an ID selector by writing a hash symbol (`#`) followed by a set of characters (the "id name").  The rule will apply to any HTML element that has an attribute `id` set with the same value of the selector (without the `#` symbol).

For example:

```css
#wrapper{
	width: 800px;
}
```

This CSS would match HTML as follows:

```html
<div id="wrapper">
…
</div>
```

The element in this case doesn’t matter; it could be a `p` or a `main`.  As long as the ID name matches the same as our rule (`wrapper`).

ID attributes should only be used once on a page.  If you apply the same ID name to multiple elements, the styles will work correctly, but the HTML will not validate.

IDs also have very high specificity - which makes it difficult to override them with other styles.

<div class="callout">
<p><strong>A note about specificity</strong></p>
<p>Specificity can be a difficult aspect of CSS to understand.  Even after writing CSS for years, I still sometimes struggle with tricky specificity and inheritance issues.</p>
<p>Here is a <a href="http://css-tricks.com/specifics-on-css-specificity/">great article from CSS Tricks</a> that helps to explain specificity.  If you’re getting confused, don’t stress.  No one will ever be quizzing you on the exact numerical specificity of a selector.  You should just understand that some selectors are more specific than others, and these selectors will override the less specific ones</p>
</div>

### Class Selector

Class selectors are very useful, and can be used in many different ways to hook styles to content.  A class selector is written by writing a dot (a period) followed by a set of characters (the class name).  The rule will apply to any HTML element that has the attribute `class` set with the same value of the selector (without the `.` symbol).

For example:

```css
.highlight{
	padding: 10px;
	border: 3px dotted black;
}
```

This CSS will match the HTML as follows:

```html
<div class="highlight">
..
</div>
```

The same styles will apply to other html elements using this class.  Reusing classes is beneficial - you don’t have to repeat yourself when writing your css!

One useful thing about classes is that you can apply multiple classes to a single HTML element.  For example:

```css
.highlight{
	padding: 10px;
	border: 3px dotted black;
}
.success-highlight{
	background-color: green;
}
.warning-highlight{
	background-color: red;
}
```

You would use this css for the following HTML .. note the multiple CSS classes separated by spaces in the class attribute.

```html
<div class="highlight success-highlight">
..
</div>

<div class="highlight warning-highlight">
..
</div>
```

## New Ways To Write Selectors

So far, we have looked at three ways to write selectors.

1) Element selectors (type selectors)

```
p { color: green; }
```

2) ID selectors

```
#wrapper{ width: 800px; }
```

3) Class selectors

```
.highlight{ color: yellow; }
```

It may become useful to combine these techniques to make your CSS more specific.  For example, you may want to target only paragraphs within your header, or links within your sidebar.

To layer selectors, simple write them on the line next to each other in your ruleset.  Add spaces between the selectors.

```css
.sidebar a{
  color: purple;
}
```

Spacing is very important.  Without adding spaces, you can target *element-specific* classes ... for example, *paragraph elements with the style highlight*.  By doing this, other elements with the style highlight would not get the styling.

```css
p.highlight{
  color: yellow;
}
```

<div class="callout">
<p><strong>Note</strong></p>
<p>A great visual example of the effect spacing has in CSS can be found at <a href="http://css-tricks.com/whats-the-difference/">CSS Tricks</a></p>
</div>

## Centering Things with CSS

One of the first things that I've noticed that you are starting to try with your styles is **centering** (with varying degrees of success). Centering is a common task in CSS.

### Centering Lines of Text

This is the most common - and the easiest - type of centering.  The CSS is as follows:

```css
p{
  text-align: center;
}
h1{
  text-align: center;
}
header{
  text-align: center;
}
```

With this styling, the text in the selected element will be centered between its margins.

You may wish to target certain portions of a site to be centered - for example, you might want your h1 and h2 in your header to be centered, but not your h1 or h2 on the rest of the site.

```html

<style>
header h1{
  text-align: center;
}
.site-subtitle{
  text-align: center;
}
</style>
...

<header>
  <h1>This text will be centered!</h1>
  <h2>This text will not be centered.</h2>
</header>

<h1>This text will not be centered.</h1>
<h2 class="site-subtitle">This text will be centered</h2>

```

### Centering Blocks

Sometimes you don't want the text _within_ a block to be centered, you want the _actual block_ to be centered on the page.  We can accomplish this by making sure of the two following things:

- the block must have a set width (be less than the width of the page, or the width of the parent element)
- the block must have equal left and right margins

We can set the left and right margins to be equal by using the following code:

```css
.branding {
  width: 800px;
  margin-left: auto;
  margin-right: auto;
}
```

## In-Class Activity - Centering Blocks

<div class="activity">
{% capture my_include %}{% include activities/15centeringblocks.md %}{% endcapture %}
{{ my_include | markdownify }}
</div>

## Homework

1. Make sure your project-portfolio index.html has the following features:
  - a list of your current projects with links to each of the project pages
  - color squares with your color scheme (review the [in-class activity](/lessons/2014-09-19.html) where we built this - I've rewritten it to be easier to follow if you missed it).
2. When we were writing our color squares, we repeated an awful lot of CSS, didn't we! See if you can make this more modular / less repetative.  **There are multiple solutions to this problem** - please come prepared to share your ideas!
3. Read Chapter 14 in your Learning Web Design book.


## Lesson Credits

- Much of the review of CSS Selectors from [Sitepoint's excellent tutorial](http://www.sitepoint.com/web-foundations/css-selectors/).