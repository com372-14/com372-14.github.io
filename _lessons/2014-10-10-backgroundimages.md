---
layout: post
title: Background Images
lesson_num: '20'
week_num: 7
class_date: October 10, 2014
lead: 
dontlink: false
---

## Due For This Class

1. Read Chapter 13 in your web design book.
2. Read the articles from the lesson
  - [Icon Usability on Nielsen](http://www.nngroup.com/articles/icon-usability/)
  - [Use and Abuse of Icons in the Modern Age](http://webdesign.tutsplus.com/articles/use-and-abuse-of-icons-in-the-modern-age--webdesign-17064)
  - [UX Myths - Myth #13: Icons enhance usability](http://uxmyths.com/post/715009009/myth-icons-enhance-usability)
  - [Why And How To Use Icon Fonts](http://www.vanseodesign.com/web-design/icon-fonts/)
3. Don't forget to submit your CodeCademy that was due Wednesday.

## Lesson Breakdown

1. Happy Birthday, CSS!
2. Beyond `background-color` - using background images


## CSS is 20!

- [The original proposal](http://www.w3.org/People/howcome/p/cascade.html)
- [Recent interview with the person who first proposed CSS](https://dev.opera.com/articles/css-twenty-years-hakon/)

<p data-height="268" data-theme-id="0" data-slug-hash="JrGxp" data-default-tab="result" data-user="sonu" class='codepen'>See the Pen <a href='http://codepen.io/sonu/pen/JrGxp/'>Birthday Cake</a> by Sonu Joshi (<a href='http://codepen.io/sonu'>@sonu</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//codepen.io/assets/embed/ei.js"></script>

## Background Images

The `background-image` property in CSS allows you to place any image behind the content of an HTML element.  A `background-image` can be applied to almost any element (not just the whole page), and by default will repeat itself to fill the entire box.

When writing your CSS to include your background image, you want to use the structure `url('path/to/img.png');`.

```css
body{
  background-image: url('../images/mybackground.png');
}
```

[View an example](../lesson_files/background-practice1.html)

If you don't want your background image to repeat, you can set that as so:

```css
body{
  background-image: url('../images/mybackground.png');
  background-repeat: no-repeat;
}
```

[View an example](../lesson_files/background-practice2.html)


You can still have a background color if you're using a background image.  You can also position the background image in a different spot (rather than the top left corner).

```css
body{
  background-color: green;
  background-image: url('seamless-bg.jpg');
  background-repeat: no-repeat;
  background-position-x: 100%;
  background-position-y: 50px;
}
```

[View an example](../lesson_files/background-practice3.html)

## In-Class Activity - Adding Social Links to your Project Portfolio

<div class="activity">
{% capture my_include %}{% include activities/20backgroundimages.md %}{% endcapture %}
{{ my_include | markdownify }}
</div>



## Homework

- Start working on [Project #5](../projects/05-resume.html).  This is due **next Friday** (Friday, October 17, 2014).
- Start working on [CSS: An Overview](http://www.codecademy.com/courses/web-beginner-en-TlhFi) (Due Wednesday, October 15, 2014)
- Start working on [Project: Design a Button for your Website](http://www.codecademy.com/courses/web-beginner-en-UuBLw) (Due Wednesday, October 15, 2014)