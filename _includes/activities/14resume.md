

<div class="activity">

<ol>
<li>In your project-portfolio folder, create a new file and name it <strong>resume.html</strong>.  Open this file and begin editing it.</li>
<li>Create the basic structure of an HTML document
    <div class="note">
    <h3>How?</h3>
    <p>Remember, you can go to our <a href="/resources">resources</a> page and use the <a href="https://github.com/com372-14/page-template">"Basic HTML Template"</a></p>
    </div>
</li>
  
<li>In the css folder of your project-portfolio, create a new stylesheet to use on your resume.  Name it <strong>resume.css</strong></li>
<li>Link your <strong>resume.css</strong> to your <strong>resume.html</strong>.
  <div class="note">
    <h3>How?</h3>
    <p>Place the following code in the <code>&lt;head&gt;</code> of your document</p>
    <pre><code class="language-html" data-lang="html"><span class="nt">&lt;link</span> <span class="na">rel=</span><span class="s">"stylesheet"</span> <span class="na">href=</span><span class="s">"css/resume.css"</span><span class="nt">&gt;</span>
  </code></pre>
  </div>
</li>

<li>Take a look at your printed resume.  Think about how you could code this.  What elements would be your headings?  What elements would be lists?  Using a pencil or pen, do some basic markup on your printed resume.</li>

<li>Still using your printed resume - are there specific sections?  For example, do you see a clear header, a footer (maybe not), areas that seem to belong together?  Think of how you could mark the content in these sections to allow them to be styled in a special way.
  <div class="note">
    <h3>How?</h3>
    <p>We can use html to mark up sections, using </p>
    <p><code>&lt;div&gt;</code>, <code>&lt;header&gt;</code>, <code>&lt;footer&gt;</code>, <code>&lt;article&gt;</code>, <code>&lt;section&gt;</code>, <code>&lt;aside&gt;</code></p>
    <p>Read more about semantic elements at <a href="http://alistapart.com/article/previewofhtml5">A List Apart</a> or <a href="http://blog.teamtreehouse.com/use-html5-sectioning-elements">Team Treehouse</a></p>
    <pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"education"</span><span class="nt">&gt;</span>
  <span class="nt">&lt;h2&gt;</span>Education<span class="nt">&lt;/h2&gt;</span>
  <span class="nt">&lt;ul&gt;</span>
    <span class="nt">&lt;li&gt;</span>Saint Joseph's University, 2010<span class="nt">&lt;/li&gt;</span>
    <span class="nt">&lt;li&gt;</span>Fairfield University, 2006<span class="nt">&lt;/li&gt;</span>
  <span class="nt">&lt;/ul&gt;</span>
<span class="nt">&lt;/div&gt;</span>
</code></pre>
  </div>

</li>

<li>Once you are happy with how it looks, begin creating styles for your resume.  At the very least, add a background color and color your h1, h2, h3, h4... tags</li>

<li>Save and add a link to this in your main project portfolio page</li>
</ol>


</div>
