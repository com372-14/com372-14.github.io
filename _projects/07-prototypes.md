---
layout: project
title: Project 7 - Prototypes
duedate: Monday, November 10, 2014
---

## Project Goals

This week you should start thinking about the design of your personal website. 

  - What do you want to build? 
  - What should it include? 
  - What kind of layout(s) might it include?

Specifically, your task: Develop prototypes for at least four pages of your personal site. You can build these with Balsamiq, with graph paper, or with any other medium of your choosing.

## Submission

1. Create your prototypes and save them as four images.  If you sketched your prototypes, scan them or take photos of them.
2. Create a new page in your project portfolio.  Name it 07prototypes.html
3. Add your four images to your images folder.
4. Each image should be placed in your prototype page.  You should scale the images (create thumbnails / utilize CSS) so that the images are viewable without being too large for the page.
5. Add styling to your page.  You can utilize Bootstrap if you would like, or use your style.css that you have used throughout the project portfolio.
6. If you do not use Bootstrap, don't forget to add a CSS Reset / Normalize file to your page. 
7. Link each image on your prototype page to the image file itself.
    
    ```html
    .... html ....
    
    <a href="images/myimage.jpg">
      <img src="images/myimage.jpg" class="scaled-image" alt="Prototype 1">
    </a>
    
    ... css ...
    
    .scaled-image{
      max-width: 100%;
      height: auto;
    }
    ```

Link this file to your main project portfolio page, and commit / sync your changes to GitHub.  **Don't forget to validate!**

## Need inspiration?

<ul>
<li><a href="http://css-tricks.com/gallery/">CSS Tricks Gallery</a></li>
<li><a href="http://www.smashingmagazine.com/portfolio-web-design-showcases/">Smashing Magazine Web Design Showcases</a></li>
<li><a href="http://sixrevisions.com/category/design-showcase-inspiration/">Six Revisions Showcase</a></li>
<li><a href="http://www.siteinspire.com/websites?categories=19">Site Inspire</a></li>
<li><a href="http://onepagelove.com/">One Page Love</a></li>
<li><a href="https://dribbble.com/">Dribbble</a></li>
<li><a href="http://tympanus.net/codrops/category/blueprints/">CoDrops BluePrints</a></li>
</ul>

## Wireframe / Prototype Tools

Choose any of these tools to create your prototypes.  Or, you can use whatever tool you wish.

- https://moqups.com/
- https://balsamiq.com/
- https://gomockingbird.com/
- https://wireframe.cc/

For a good guide on wireframing, you can read [this article from TutsPlus](http://webdesign.tutsplus.com/articles/a-beginners-guide-to-wireframing--webdesign-7399)