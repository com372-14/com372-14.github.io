1. Create an account on [Codepen](https://codepen.io/login) (you can use your github account to login!)
2. Create a new pen
3. In the bottom right-hand corner, you'll see three buttons - for "HTML", "CSS", and "JS".  Click the "JS" one (we aren't using Javascript so we can hide this)
4. In the HTML section, create a heading (h1, h2, etc) and put some text in it.
5. In the CSS section, give your `body` a background color.
6. In the CSS section, set your heading to a larger font size.  Give it a color.  
7. Let's try to change the color when we hover over the heading (the following instructions assume you're using `h1`)
  - create a new rule.  The selector should be `h1:hover`
  - inside the rule, set the color to a different color than your normal text.
  - try it out!  the text should change color!

## Using Google Web Fonts in CodePen

You can use Google Web Fonts in Codepen. Just go to Google fonts, pick a font, and use the `@import` version of the font (the second tab in the 'use' section).  Put this at the top of your CSS.

```
@import url(http://fonts.googleapis.com/css?family=Kavoon);
```

## Fading!

1. When we hover our text, it makes it immediately the new color.  What if we wanted to make it a different color slowly?
2. We can use `transition`.  Transition lets us affect the things that happen if the element changes (for example, when you hover).  There are lots of reasons an element might change - the one we are using now is when you hover over something.

```
.example {
    transition: [transition-property] [transition-duration] [transition-timing-function] [transition-delay];
}
```

We want to set the color to change slowly by using the following code

```
h1 {
  transition: color 1s;
}
```

[Read more about transitions](http://css-tricks.com/almanac/properties/t/transition/)

## Text Shadow

8. Let's try to add a text-shadow.
  - inside the normal h1 rule, add a new property
  - the property name is `text-shadow`.
  - there are four values - three numbers and a color.
  - the first number is the x-offset.  the second number is the y-offset.  the third number is the blur.  the color is any CSS color (including rgba - for semi-transparent colors)
  - your final property should look something like this
  <div class="highlight"><pre><code class="language-text" data-lang="text">  h1{
      ...
      text-shadow: 4px 10px 5px #167DAD;
    }
  </code></pre></div>


## Circles!

9. Let's try to make a circle.  First, make a box - create an empty div and give it a class.
<div class="highlight"><pre><code class="language-text" data-lang="text">  &lt;div class="circle"&gt;&lt;/div&gt;
</code></pre></div>

10. In your CSS, give your circle a background color, and a width and a height.  Set it so it's centered in the window
<div class="highlight"><pre><code class="language-text" data-lang="text">  .circle{
    background-color: orange;
    width: 150px;
    height: 150px;
    margin: 0px auto;
  }
</code></pre></div>

## Glowing!

1. Let's make our circle glow!
2. We can add shadow to boxes too - not just text.
3. In your CSS, in the style for the circle, set the `box-shadow` with a shadow that has no offset (the first two numbers will be 0), and a lot of blur.  Set the color to yellow (or any other color that will stand out on your page)

## Growing!

1. We can use CSS to make things bigger and smaller.
2. Let's make our circle bigger when we hover it.

```
.circle:hover{
  transform: scale(3);
}
```

Well, that's a sudden change!  Let's add a timing to that transition to slow it down a bit!  Remember, our transition goes in the CSS for the original element (not the hover)

```
.circle {
  ..
  transition: transform 1s;
}
```

[Read more about transform and the things you can do!](http://css-tricks.com/almanac/properties/t/transform/)