1. Go to [pexels](http://www.pexels.com) and find a background photo you want to use.  Try to find something that you will be able to lay either white or black text over and there will be enough contrast for you to read the text.
2. Download this file and place it in the "images" folder in your project portfolio.
3. Create a new file in your project porfolio and name it `splash.html`.  Copy the code from our [project-template](https://github.com/com372-14/project-template/blob/master/index.html) into it.
4. Create a new file in your CSS folder and name it `splash.css`.
5. If you don't have normalize in your CSS folder, [download it from here](https://github.com/com372-14/project-template/blob/master/css/normalize.css) and save it to your css folder. 
6. At the top of the `splash.html` there is a link for `css/style.css`.  Change this to `css/splash.css`.
7. Create a div as the first part of the `body`, and set the class as `page-wrap`
  
  ```
  <div class="page-wrap">
  
  </div>
  ```
  
8. Create a ul as the first part of the page-wrap, and set the class to `social`.
9. Create at least two list items.  Use Font Awesome to create social icons.  Review step 5 in [last week's activity](http://com372-14.github.io/lessons/2014-10-08-typeandnavigation.html) if you forget how to do this.
10. Under the ul, create an H1 and an H2.  Set the text of the H1 to your name, and the text of the H2 to a short statement about you.
11. Live preview!  You should have a list on the page and two headings.
12. Open your ``css/splash.css``.
13. At the top, add a cover-sized background image.  You can get the code from [CSS Tricks](http://css-tricks.com/perfect-full-page-background-image/)

```
html { 
  background: url(images/bg.jpg) no-repeat center center fixed; 
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
```








6. Add a background image to the `body`.  There is an image you can use in the `img` folder.  To do so, add the following to your CSS.
<div class="note">
Add the following to the **style.css** that is in your CSS folder.
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">body</span><span class="p">{</span>
  <span class="k">background-image</span><span class="o">:</span> <span class="sx">url('../img/balloons.png')</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>
</div>

7. That makes our text really hard to read, doesn't it?  Add a background color to your header, footer, and .birthday-message to make the text easier to read!