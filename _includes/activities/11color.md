1. Open your **project-portfolio** in Brackets.  We will be editing your *index.html* file, so double-click to open that and edit it.
2. Create a new folder in your project and name it `css`.  Create a new file in this folder, and name it *style.css*.
3. Link your **style.css** file to your **index.html** file.
<div class="note">
<p><strong>How?</strong></p>
<p>Place the following code in the <code>head</code> of your document</p>
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;link</span> <span class="na">rel=</span><span class="s">"stylesheet"</span> <span class="na">href=</span><span class="s">"css/style.css"</span><span class="nt">&gt;</span>
</code></pre></div>
</div>

4. Open your **style.css** file.
5. Create a comment at the top of your CSS file.  Write your name, and then put the hex codes for your three colors in the comment (this will help you to reference them later).
<div class="note">
<p><strong>How?</strong></p>
<p>Remember, the comment structure for CSS is as follows:</p>
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="c">/* </span>
<span class="c">Start your comment with a backslash followed by a star.</span>
<span class="c">End your comment with a star followed by a backslash.</span>
<span class="c">Everything between is your comment!</span>
<span class="c">*/</span>
</code></pre></div>
</div>

6. Choose one of your colors, preferably one that is highly saturated.
7. Using CSS, set this to be the color of all your links and h1's.  You want to write these styles in your CSS file.
<div class="note">
<p><strong>How?</strong></p>
<p>In this example, we are using #990000 as our color.  You would use your own color code!</p>
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">a</span><span class="p">{</span>
  <span class="k">color</span><span class="o">:</span> <span class="m">#990000</span><span class="p">;</span>
<span class="p">}</span>
<span class="nt">h1</span><span class="p">{</span>
  <span class="k">color</span><span class="o">:</span> <span class="m">#990000</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>
<p>We are using <code>a</code> and <code>h1</code> as our <strong>selectors</strong>, because we want to apply the styling to all elements on the page that match those selectors.</p>
</div>

8. Add another CSS rule, this time using `h2` as your selector.  Set the color of the `h2` to one of your other colors.
9. Let's make sure that our **index.html** has markup that will match our styling.  Edit your **index.html**.  At the beginning of the file, directly after your ``<body>`` tag, create a h1 and make sure that it has your name and "Project Portfolio".
10. Create an h2 under that and make the content "Classwork and Projects for COM372"
11. Add a paragraph of text under that.  Write whatever you want.  You can search google for Random Text and get a block of random text.
<div class="note">
<p><strong>Your index.html should now have at least the following content.</strong></p>
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="cp">&lt;!DOCTYPE html&gt;</span>
<span class="nt">&lt;html&gt;</span>
  <span class="nt">&lt;head&gt;</span>
    <span class="nt">&lt;title&gt;</span>MYNAME Project Portfolio<span class="nt">&lt;/title&gt;</span>
    <span class="nt">&lt;link</span> <span class="na">rel=</span><span class="s">&quot;stylesheet&quot;</span> <span class="na">href=</span><span class="s">&quot;css/style.css&quot;</span><span class="nt">&gt;</span>
  <span class="nt">&lt;/head&gt;</span>
  <span class="nt">&lt;body&gt;</span>
    <span class="nt">&lt;h1&gt;</span>MYNAME&#39;s Project Portfolio<span class="nt">&lt;/h1&gt;</span>
    <span class="nt">&lt;h2&gt;</span>Classwork and Projects for COM372<span class="nt">&lt;/h2&gt;</span>
    <span class="nt">&lt;p&gt;</span>A paragraph of random text<span class="nt">&lt;/p&gt;</span>
    ..... <span class="c">&lt;!-- you shouldn&#39;t have dots here, this is just a note to show the page goes on--&gt;</span>
  <span class="nt">&lt;/body&gt;</span>
<span class="nt">&lt;/html&gt;</span>
</code></pre></div>
</div>

12. Under the paragraph, create a three new paragraphs.  As the content for each one, write your hex codes for your colors.  You can add descriptions to your colors
<div class="note">
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;p&gt;</span>A paragraph of random text<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p&gt;</span>Red - #990000<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p&gt;</span>Purple - #3D2040<span class="nt">&lt;/p&gt;</span>
<span class="nt">&lt;p&gt;</span>Yellow - #FFCF40<span class="nt">&lt;/p&gt;</span>
</code></pre></div>
</div>

13. Surround each of the three paragraphs with a `<div>`.
<div class="note">
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;div&gt;&lt;p&gt;</span>Red - #990000<span class="nt">&lt;/p&gt;&lt;/div&gt;</span>
<span class="nt">&lt;div&gt;&lt;p&gt;</span>Purple - #3D2040<span class="nt">&lt;/p&gt;&lt;/div&gt;</span>
<span class="nt">&lt;div&gt;&lt;p&gt;</span>Yellow - #FFCF40<span class="nt">&lt;/p&gt;&lt;/div&gt;</span>
</code></pre></div>
</div>

14. Create styles for your divs.  We want to make them squares and give them background colors.  In your `style.css`, write the following styles.  Instead of using the sample background color, use one of your colors!
<div class="note">
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">div</span><span class="p">{</span>
  <span class="k">width</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">height</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">background-color</span><span class="o">:</span> <span class="m">#990000</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>
</div>

15. Save your `index.html` and your `style.css`, and open your `index.html` using livepreview.  You should see that your divs have changed - they will all have the same background color!
16. We don't want all our divs to have the SAME background color, we want them to have background colors that represent our color scheme.  Let's use classes to help us accomplish this.
17. Edit your index.html.  Add classes to each of your divs.  The classes should be: `color1`, `color2`, `color3`.
<div class="note">
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"color1"</span><span class="nt">&gt;&lt;p&gt;</span>Red - #990000<span class="nt">&lt;/p&gt;&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"color2"</span><span class="nt">&gt;&lt;p&gt;</span>Purple - #3D2040<span class="nt">&lt;/p&gt;&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"color3"</span><span class="nt">&gt;&lt;p&gt;</span>Yellow - #FFCF40<span class="nt">&lt;/p&gt;&lt;/div&gt;</span>
</code></pre></div>
</div>

18. We want to change our selector in CSS to apply to these classes instead of to the element `div`.  Edit your CSS rule to have `.color1` as the selector instead of `div`.
<div class="note">
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nc">.color1</span><span class="p">{</span>
  <span class="k">width</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">height</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">background-color</span><span class="o">:</span> <span class="m">#990000</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>
</div>

19. Save your `index.html` and your `style.css`, and open your `index.html` using livepreview.  You should see that your divs have changed - only the first one is styled now!
20.  We will need to repeat our styling so that it can be applied to the other divs.
21.  Copy your rule set (from the . that starts the selector all the way through the closing }) and paste it into your CSS twice.  You should now have three rulesets, all with the selector `.color1`.  Change the second selector to `.color2` and the third selector to `.color3`.  Then, take your two other colors and use them for the background color for the two new rulesets.
<div class="note">
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nc">.color1</span><span class="p">{</span>
  <span class="k">width</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">height</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">background-color</span><span class="o">:</span> <span class="m">#990000</span><span class="p">;</span>
<span class="p">}</span>
<span class="nc">.color2</span><span class="p">{</span>
  <span class="k">width</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">height</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">background-color</span><span class="o">:</span> <span class="m">#3D2040</span><span class="p">;</span>
<span class="p">}</span>
<span class="nc">.color3</span><span class="p">{</span>
  <span class="k">width</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">height</span><span class="o">:</span> <span class="m">200px</span><span class="p">;</span>
  <span class="k">background-color</span><span class="o">:</span> <span class="m">#FFCF40</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>
</div>