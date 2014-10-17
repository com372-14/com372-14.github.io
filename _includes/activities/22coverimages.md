1. Go to [pexels](http://www.pexels.com) and find a background photo you want to use.  Try to find something that you will be able to lay either white or black text over and there will be enough contrast for you to read the text.
2. Download this file and place it in the "images" folder in your project portfolio.
3. Create a new file in your project porfolio and name it `splash.html`.  Copy the code from our [project-template](https://github.com/com372-14/project-template/blob/master/index.html) into it.
4. Create a new file in your CSS folder and name it `splash.css`.
5. If you don't have normalize in your CSS folder, [download it from here](https://github.com/com372-14/project-template/blob/master/css/normalize.css) and save it to your css folder.
6. At the top of the `splash.html` there is a link for `css/style.css`.  Change this to `css/splash.css`.
7. Create a div as the first part of the `body`, and set the class as `page-wrap`
<div class="highlight"><pre><code class="language-text" data-lang="text">  &lt;div class="page-wrap"&gt;
    &nbsp;
  &nbsp;&nbsp;&lt;/div&gt;
</code></pre></div>
  
8. Create a `ul` as the first part of the page-wrap, and set the class to `social`.
9. Create at least two list items.  Use Font Awesome to create social icons.  Review step 5 in [last week's activity](http://com372-14.github.io/lessons/2014-10-08-typeandnavigation.html) if you forget how to do this.
10. Under the ul, create an `H1` and an `H2`.  Set the text of the H1 to your name, and the text of the H2 to a short statement about you.
11. Hit enter a few times, and then go into the website HTML-Ipsum and copy the ["Kitchen Sink"](http://html-ipsum.com/) text.  Paste it into your document.  This is just to make the page longer. 
11. Live preview!  You should have a list on the page and two headings, plus the random text from HTML-Ipsum
12. Open your ``css/splash.css``.
13. At the top, create a CSS rule that will apply to the **entire html document**.  Add a background image.  The image will be the photo you downloaded from pexels.
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">html</span><span class="p">{</span>
  <span class="k">background-image</span><span class="o">:</span> <span class="sx">url(images/my-image.jpg)</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>

14. Live preview.  What happened?  Is your photo too big for your browser and you are only seeing a part of it?  Or maybe your photo is too small and it's repeating.  First, let's make it stop repeating.
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">html</span><span class="p">{</span>
  <span class="k">background-image</span><span class="o">:</span> <span class="sx">url(images/my-image.jpg)</span><span class="p">;</span>
  <span class="k">background-repeat</span><span class="o">:</span> <span class="k">no-repeat</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>

15. Now, position it.  The position takes two attributes - one for x axis and one for y axis.  We can use pixels, percentages, or just "top", "center", "left", "right" or "bottom".  We will be using **center center** to position the background image in the center of our document.
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">html</span><span class="p">{</span>
  <span class="k">background-image</span><span class="o">:</span> <span class="sx">url(images/my-image.jpg)</span><span class="p">;</span>
  <span class="k">background-repeat</span><span class="o">:</span> <span class="k">no-repeat</span><span class="p">;</span>
  <span class="k">background-position</span><span class="o">:</span> <span class="k">center</span> <span class="k">center</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>

16. Backgrounds can also be attached to the window - you can have them fixed in place, or you can have them scroll.  We want ours fixed in place.
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">html</span><span class="p">{</span>
  <span class="k">background-image</span><span class="o">:</span> <span class="sx">url(images/my-image.jpg)</span><span class="p">;</span>
  <span class="k">background-repeat</span><span class="o">:</span> <span class="k">no-repeat</span><span class="p">;</span>
  <span class="k">background-position</span><span class="o">:</span> <span class="k">center</span> <span class="k">center</span><span class="p">;</span>
  <span class="k">background-attachment</span><span class="o">:</span> <span class="k">fixed</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>

17. Now for the magic.  Let's make this image fit in the space we have for it!
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">html</span> <span class="p">{</span> 
  <span class="k">background-image</span><span class="o">:</span> <span class="sx">url(images/my-image.jpg)</span><span class="p">;</span>
  <span class="k">background-repeat</span><span class="o">:</span> <span class="k">no-repeat</span><span class="p">;</span>
  <span class="k">background-position</span><span class="o">:</span> <span class="k">center</span> <span class="k">center</span><span class="p">;</span>
  <span class="k">background-attachment</span><span class="o">:</span> <span class="k">fixed</span><span class="p">;</span>
  <span class="k">background</span><span class="o">-</span><span class="k">size</span><span class="o">:</span> <span class="n">cover</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>

18. Let's live preview!