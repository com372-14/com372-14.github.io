---
layout: post
title: Typography and Navigation
lesson_num: '19'
week_num: 7
class_date: October 8, 2014
lead: 
dontlink: false
---

## Homework

- Read two sections from [Butterick’s Practical Typography](http://practicaltypography.com/)
  - [Typography in Ten Minutes](http://practicaltypography.com/typography-in-ten-minutes.html)
  - [Summary of Key Rules](http://practicaltypography.com/summary-of-key-rules.html)
  
- Read Chapter 12 of your Web Design book.
- Find at least five websites that you think have good type.  Add them to your inspiration journal.  Explain what you like about each site.  Share your inspiration journal with me!
- Complete the next two lessons in CodeCademy
  *  [HTML Basics III](http://www.codecademy.com/courses/web-beginner-en-f8mcL) (Due Wednesday, October 8, 2014)
  *  [Project: Clickable Photo Page](http://www.codecademy.com/courses/web-beginner-en-zrZ6c) (Due Wednesday, October 8, 2014)

## Lesson

1. Questions about type
2. Icon fonts
3. Pseudo-classes / Hovering things
4. In-Class Activity

## Icon Fonts

[Why are Icon Fonts Awesome?](http://css-tricks.com/examples/IconFont/)

Icons are great for providing a little bit of extra visual meaning to your content.  They can provide visual interest, and allow for easier communication with your audience.

The overuse of icons should be avoided, and you should take care that your icons are communicating the correct meaning to the audience.  Text labels should accompany icons when possible.

Here are four articles about icon usability

- [Icon Usability on Nielsen](http://www.nngroup.com/articles/icon-usability/)
- [Use and Abuse of Icons in the Modern Age](http://webdesign.tutsplus.com/articles/use-and-abuse-of-icons-in-the-modern-age--webdesign-17064)
- [UX Myths - Myth #13: Icons enhance usability](http://uxmyths.com/post/715009009/myth-icons-enhance-usability)
- [Why And How To Use Icon Fonts](http://www.vanseodesign.com/web-design/icon-fonts/)

### How to Use Icons

Traditionally, images have been used as icons on the web.  If you visit sites like [IconFinder](https://www.iconfinder.com/) or simply google "web icons" you will find lots of different icons that you can use in your designs.  These types of icons would be included on your site exactly like you would include an image.

```html
<a href="http://www.facebook.com">
  <img src="img/fbicon.png" alt="Facebook Icon" />
</a>
```

<a href="http://www.facebook.com"><img src="/lesson_files/facebooksheep.png" alt="Facebook Icon" width="64" height="64" /></a>

### Alternate - using image fonts

Using image as icons has lots of pros (you can get really custom with your icons, do cool things), but also some drawbacks.  What if you want a larger icon?  You would have to find some way to enlarge your image.  What if you want to change the color?  You would have to recreate your image.

With modern browsers we have the option of using icon fonts.  Icon fonts allow you to highly customize your icons, changing size and color - they act a lot like text on your website!

### Using Icon Fonts

I like using FontAwesome for my icon fonts.  I find that most of the icons I want to use are included, and it's really easy to add to projects.  You'll see that we actually use these in the Nest, and on some of SJU's other websites.

[FontAwesome](http://fontawesome.io/)

You can use FontAwesome without having to download anything. Simply follow the instructions on FontAwesome's site.

### Custom Icon Fonts

Using a library like FontAwesome is awesome, because it's all built right for you.  If you are only using a few icons, or you want to create your own icon set, you may wish to use a service like [IcoMoon](http://www.icomoon.io).  A great tutorial that leads you through this process (including creating your own font, downloading the files, and including them in your website) is available on [Go Make Things](http://gomakethings.com/icon-fonts/).

## CSS Pseudo Classes

So far we have been using CSS selectors like the following:

```css

ul { .. } /* Type or Element Selector */

.myclass { .. } /* Class Selector */

#mainheader { .. } /* ID Selector */

```

We've also learned that we can combine selectors, like so:

```css

header.main { .. } /* This will target the element header with the class of main, so <header class="main"> */

.myclass a { .. } 

/* This will target all the links that are descendants of .myclass  
    <div class="myclass">
      <p>This text will be <a href="#">styled</a></p>
    </div>
*/

```

Another way we can use CSS is to talk about specifics of an element.  So, you may have seen something like this before

```css
a:link, a:visited {
	color: blue;
}
```

The :link and :visited that are stuck to the selector (in this case, **a**) are called **pseudo classes**.  Pseudo classes are used to be more specific about how you want your CSS to appy, and when.

A great use-case for this is to change link styling when you hover over the link.

For example, we may have CSS that's as follows:

```css
.example a {
	font-size: 2em;
	color:green;
	text-decoration: none;
}
```

And the result is:

<style>
.example a, .example a:hover {
	font-size: 2em;
	color:green;
	text-decoration: none;
	border-bottom: 0;
	opacity: 1;
}
</style>
<span class="example">
  <a href="#">This is my link</a>
</span>

But let's say that when the user hovers over it, we want it to change in some way.  For example, we may want to underline, or change the color.  Let's do both.

We do this by using the :hover pseudo class.  When we stick :hover right onto the selector, we're saying "Hey, apply this CSS when I'm hovering over this thing!"

```css
.example a:hover {
	color: blue;
	text-decoration: underline;
}
```

And the result is:

<style>
.example a:hover {
	color: blue;
	text-decoration: underline;
}
</style>
<span class="example">
  <a href="#">This is my link</a>
</span>


## In-Class Activity - Adding Social Links to your Project Portfolio

<div class="activity">
{% capture my_include %}{% include activities/19iconsandpseudoclasses.md %}{% endcapture %}
{{ my_include | markdownify }}
</div>

## Homework

1. Read Chapter 13 in your web design book.