---
layout: project
title: Project 3 - Placing Images
duedate:
---

## Time Needed

Approximate Time needed : 1 - 2 hours (including reading and searching for photos)

## What You'll Learn

This project should help you get familiar with putting images into websites, and the proper file formats for a given situation.

## Read Me First

- Chapter 9, White Space is Not Your Enemy (pg 136 - 158)
- Chapter 7, Learning Web Design (pg 123-132)

## What You'll Produce

You will project an HTML web page with multiple images.  These images can be either personal images, or images found on the internet.

**Please use at least one photo you have found on the internet**. If you are using photos found on the internet, be sure that they are not copyrighted.  Read [more about copyright and internet images](http://www.socialmediaexaminer.com/copyright-fair-use-and-how-it-works-for-online-images/).

Dustin Senos has curated a [list of great places to get stock photography](https://medium.com/@dustin/stock-photos-that-dont-suck-62ae4bcbe01b) without having to pay for it.  Please be sure to **pay attention** to licensing (frequently you will see references to [Creative Commons licensing](http://creativecommons.org/licenses/)).

## Step-By-Step Instructions

- Create a new html file and name it 03photos.html
- In the root folder of your Project Portfolio, create a new folder and call it images (or img)
- In this newly created Images folder, create another folder and name it "project3"
- Select a topic that you will base your images around (you don't have to get too fancy, just pick something to give your page cohesion).  Sample topics:
  - Old Buildings
  - Landscapes
  - Freshman Year
  - Kittens
  - Fire
- Based on your topic, find images
  Five Photographs (.jpg or .jpeg file type)
  Transparent Image (.png or .gif)
- Save your images into the "project3" folder
  - you may need to resize your images, particularly the photos.  You can use Photoshop or [Pixlr](http://pixlr.com/editor/).
  - make sure your photos do not exceed 800px by 600px 
- Create a `h1` element, setting the text of the element as your page topic
- Create two `h2` elements, the first one "Photos" and the second one "Graphics"
- After the first `h2` element, use the img tag to add your five photographs to the page
  - be sure to include the `src` attribute for each image
  - be sure to include `alt` text for each image
  - after each image, include a `<p>` element that describes the image and provides a working link to the source of the image (if needed). 
- After the second `h2` element, use the img tag to add your transparent image to the page.
- Set the body’s background to a color, anything but white using HTML,
  - Use CSS: In between the opening head and closing /head tag put the following tag:

  
```html
<style>
  body {background-color: aqua}
</style>
```
  - (if you want, you can choose another color. Choose a named color - here is a [list of named html colors](http://html-color-codes.info/color-names/).  Change the word "aqua" to any of the other colors. I reco)
  - Add a link to your new page to your Project Portfolio index.html
  
### Delivery 

When you have completed this project, commit it to your GitHub Project Portfolio repository.  Don't forget to add a link to this new page from your index.html page!


### Credit
Project inspired by Debra Kayes, Columbia College, Chicago