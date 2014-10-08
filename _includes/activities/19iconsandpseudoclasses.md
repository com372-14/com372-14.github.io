1. Open your project portfolio in Brackets.
2. Open `index.html`.
3. At the end of the file, BEFORE the `</body>`, create a new element - footer.  Add a class to your footer, called 'site-footer'
<div class="note">
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;footer class="site-footer"&gt;</span>
<span class="nt">&lt;/footer&gt;</span>
</code></pre></div>
</div>

4.  Create a list inside your footer.  Add three list items.  Make them **GitHub** and **Email**.
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;footer class="site-footer"&gt;</span>
  <span class="nt">&lt;ul&gt;</span>
    <span class="nt">&lt;li&gt;</span>GitHub<span class="nt">&lt;/li&gt;</span>
    <span class="nt">&lt;li&gt;</span>Email<span class="nt">&lt;/li&gt;</span>
  <span class="nt">&lt;/ul&gt;</span>
<span class="nt">&lt;/footer&gt;</span>
</code></pre></div>

5. At the TOP of your document, before your linked CSS file but after your `</title>` add the following line.  I got this from FontAwesome's [Getting Started](http://fontawesome.io/get-started/) page.  We are using their CDN so that we don't have to download anything separate.
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;link</span> <span class="na">href=</span><span class="s">"//maxcdn.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.min.css"</span> <span class="na">rel=</span><span class="s">"stylesheet"</span><span class="nt">&gt;</span>
</code></pre></div>

6. Go back down to the footer.  Add icons.  You can use ``<span>`` or ``<i>`` as the element to add your icons.  In this example we will use span.
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;footer</span> <span class="na">class=</span><span class="s">"site-footer"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;ul&gt;</span>
    <span class="nt">&lt;li&gt;&lt;span</span> <span class="na">class=</span><span class="s">"fa fa-github"</span><span class="nt">&gt;&lt;/span&gt;</span> GitHub<span class="nt">&lt;/li&gt;</span>
    <span class="nt">&lt;li&gt;&lt;span</span> <span class="na">class=</span><span class="s">"fa fa-envelope"</span><span class="nt">&gt;&lt;/span&gt;</span> Email<span class="nt">&lt;/li&gt;</span>
  <span class="nt">&lt;/ul&gt;</span>
<span class="nt">&lt;/footer&gt;</span>
</code></pre></div>

7. LivePreview!  Do you see the icons in your footer?
8. Now, let's link these!  After the ``<li>`` open tag, start an ``<a>``.  The href should go to your GitHub page.  Don't forget to close your ``<a>``
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;li&gt;</span>
  <span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"http://github.com/com372-14"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"fa fa-github"</span><span class="nt">&gt;&lt;/span&gt;</span> GitHub
  <span class="nt">&lt;/a&gt;</span>
<span class="nt">&lt;/li&gt;</span>
</code></pre></div>
 
9. Let's link your email.  Use mailto:MYEMAIL@EMAIL.COM as the value for href.
<div class="highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;li&gt;</span>
  <span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"mailto:MYEMAIL@EMAIL.COM"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"fa fa-envelope"</span><span class="nt">&gt;&lt;/span&gt;</span> Email
  <span class="nt">&lt;/a&gt;</span>
<span class="nt">&lt;/li&gt;</span>
</code></pre></div>

10. Save your changes.  Open your style.css
11. Create a new css rule to target the links in your footer.  Pick a font-size and a color!
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nc">.site-footer</span> <span class="nt">a</span><span class="p">{</span>
  <span class="k">font-size</span><span class="o">:</span> <span class="m">2em</span><span class="p">;</span>
  <span class="k">color</span><span class="o">:</span> <span class="nb">green</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>

12. Create a second css rule to target the links in your footer **when you hover them**.  Make them a different color!
<div class="highlight"><pre><code class="language-css" data-lang="css"><span class="nc">.site-footer</span> <span class="nt">a:hover</span><span class="p">{</span>
  <span class="k">color</span><span class="o">:</span> <span class="nb">purple</span><span class="p">;</span>
<span class="p">}</span>
</code></pre></div>

13. Save your work and commit to GitHub.

### Finished and class isn't over?

1. Add another footer link.  Link to a social media profile.  Find the icon on [FontAwesome's](http://fontawesome.io/icons/) icon page
2. What happens if you try to add :hover to another element?  Try to change the color of the text inside your color squares when you hover on them.
<style>
.solution *{
  background-color: #000;
  color: #000;
}
.solution:hover *{
  background-color: white;
}
</style>
<h4>Hover below to view the solution.</h4>
<div class="solution">
<pre><code class="language-text" data-lang="text">.color1{
  color: white;
}
.color1:hover{
  color: yellow;
}
</code></pre>
</div>

3. Try to figure out how I just did THAT (hovering to see the solution).  Don't cheat by looking at my code, since I had to use a bit of a hack to override the default styling on our course website.