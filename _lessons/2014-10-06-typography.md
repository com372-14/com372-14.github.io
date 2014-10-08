---
layout: post
title: Typography
lesson_num: '18'
week_num: 7
class_date: October 6, 2014
lead: 
dontlink: false
---

## Due For This Class

1. **Get Inspired** - start looking around on the web for things that inspire you - projects you like, screenshots of other websites, articles that interest you.  Start working on your Evernote journal.  You should continue adding to this as the semester continues.  On **October 27**, I will be asking you to write a brief overview of your journal, and another at finals.
2. Complete the next two lessons in CodeCademy
  *  [HTML Basics III](http://www.codecademy.com/courses/web-beginner-en-f8mcL) (Due Wednesday, October 8, 2014)
  *  [Project: Clickable Photo Page](http://www.codecademy.com/courses/web-beginner-en-zrZ6c) (Due Wednesday, October 8, 2014)
3. Read Chapter 5 (Mini-Art School) and Chapter 7 (Type) in White Space is Not Your Enemy.

## Typography Video

Let's watch this 5 minute video about typography. ([Click here to launch the video](https://www.youtube.com/watch?v=wOgIkxAfJsk))

## CSS Styling for Text

There are lots of ways to style text using CSS, more than we can cover just in this class.  We've gone over a lot of the basics so far.

### Color & Size

```css
.myclass{
  color: red;
  font-size: 18px;
}
```

<span style="color:red;font-size:18px;margin-left:30px;">Example text #1</span>


```css
.myclass{
  color: blue;
  font-size: 2em;
}
```

<span style="color:blue;font-size:2em;margin-left:30px;">Example text #1</span>

### Bold, italic, and underline

```css
.myclass{
  text-decoration:underline;
  font-weight:bold;
  font-style:italic;
}
```

<span style="text-decoration:underline;font-weight:bold;font-style:italic;;margin-left:30px;">No "strong" or "em" tags needed!</span>

_(although I'm showing you how to underline here, it will CONFUSE YOUR VISITORS if you underline things that are not links.  Avoid using underlines on non-linked things)__

### Transform

```css
.myclass{
  text-transform: uppercase;
}
```

<span style="text-transform: uppercase;padding-left:30px;">Stop typing things in all uppercase - use text transform!</span>


### Font Family

Font family is a great way to make your website look a little fancier / add some personality to your website.

```css
.myclass{
  font-family: sans-serif;
}
```

There are a number of generic font familys you should know.  Generic family names include `serif`, `sans-serif`, `cursive`, `fantasy`, and `monospace`.

You can also use named fonts.  Named fonts are read in the order they appear - the text will use the **first available** font from your list!  You should always include a generic font family at the end of your font stack - in case the users computer has no custom fonts installed.

You can use any font you have on your computer, but you have to be careful because people who visit your website will also need to have that font installed to see your font.  For example, open this website on your computer.  The below text on my computer looks like it is written in a casual, handwritten font, but on your computer it will probably just be cursive.

```css
.myclass{
  font-family: 'MF Be Yourself',cursive;
  font-size: 3em;
}
```
<span style="font-family:'MF Be Yourself',cursive;font-size: 3em;">A Fun Font!</span>

## Font Stacks

As you're choosing your default fonts, it's important to try to find a font that will work for the majority of your viewers.  You can do this by creating a font stack that uses fonts that most users will have installed.

There are some lists of great default font stacks at the website [CSS Font Stack](http://cssfontstack.com/).  You can read more about font stack at [Smashing Magazine](http://www.smashingmagazine.com/2009/09/22/complete-guide-to-css-font-stacks/) - and even more at [A Way Back](http://www.awayback.com/revised-font-stack/)

## Activity

Choose a default font stack for your website, and apply it to your entire page by adding the following CSS to your `styles.css`.

Don't forget to switch to your project portfolio folder!

```css
body{
  font-family: ***MY Font Stack Here***;

}
```

You can also play around with some different CSS text styling effects here -  http://csstxt.com/

## Lesson Heading
  
## Homework

- Read two sections from [Butterick’s Practical Typography](http://practicaltypography.com/)
  - [Typography in Ten Minutes](http://practicaltypography.com/typography-in-ten-minutes.html)
  - [Summary of Key Rules](http://practicaltypography.com/summary-of-key-rules.html)
  
- Read Chapter 12 of your Web Design book.
- Find at least five websites that you think have good type.  Add them to your inspiration journal.  Explain what you like about each site.  Share your inspiration journal with me!
- Complete the next two lessons in CodeCademy
  *  [HTML Basics III](http://www.codecademy.com/courses/web-beginner-en-f8mcL) (Due Wednesday, October 8, 2014)
  *  [Project: Clickable Photo Page](http://www.codecademy.com/courses/web-beginner-en-zrZ6c) (Due Wednesday, October 8, 2014)