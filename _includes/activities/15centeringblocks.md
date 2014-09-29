1. Open your **project-portfolio** in Brackets.  We will be editing your *index.html* file, so double-click to open that and edit it.
2. At the top of your **index.html** file, you should have the following code:
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
</code></pre></div>
</div>

3. You should also have a **style.css** file created in your css folder.
4. In your *index.html*, surround the `<h1>` and `<h2>` at the top of the page with a `<header>`
<div class="note">
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;header&gt;</span>
  <span class="nt">&lt;h1&gt;</span>MYNAME&#39;s Project Portfolio<span class="nt">&lt;/h1&gt;</span>
  <span class="nt">&lt;h2&gt;</span>Classwork and Projects for COM372<span class="nt">&lt;/h2&gt;</span>
<span class="nt">&lt;/header&gt;</span>
</code></pre></div>
</div>

4. Open your **style.css** file.
5. Create a style that will target the `<header>` and give it a background color of light grey (#dddddd), and a width of 800px.
<div class="note">
<p><strong>How?</strong></p>
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">header</span><span class="p">{</span>
  <span class="k">background-color</span><span class="o">:</span> <span class="m">#dddddd</span><span class="p">;</span>
  <span class="k">width</span><span class="o">:</span> <span class="m">800px</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>
</div>

6. Save your `index.html` and your `style.css`, and open your `index.html` using livepreview.  You should see that your header doesn't take up the whole width of the page anymore - but it's not centered yet!
7. Let's center the header - we want to center the **block itself**, not just the text within it.
<div class="note">
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nt">header</span><span class="p">{</span>
  <span class="k">background-color</span><span class="o">:</span> <span class="m">#dddddd</span><span class="p">;</span>
  <span class="k">width</span><span class="o">:</span> <span class="m">800px</span><span class="p">;</span>
  <span class="k">margin-left</span><span class="o">:</span> <span class="k">auto</span><span class="p">;</span>
  <span class="k">margin-right</span><span class="o">:</span> <span class="k">auto</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>
</div>

8. Save your `index.html` and your `style.css`, and open your `index.html` using livepreview.  Your header should now be centered!
