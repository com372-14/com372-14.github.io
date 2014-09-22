---
layout: default
title: Sublime Text Instructions
slug: sublimetext
---

## Sublime Text Instructions

While we have been using Brackets in class, there are lots of other great code editors out there.  Some are more full-featured than Brackets, and some are less.

Two free alternatives to Brackets are [Atom](http://www.atom.io) (created by GitHub) and [Sublime Text](http://www.sublimetext.com/).  Both of these alternatives take a little more configuration to set up than Brackets, but you may find that you like one code editor versus another.

## Installing Sublime Text

Visit the [Sublime Text Website](http://www.sublimetext.com/2) and download *Sublime Text 2*.  You will be downloading the full version - you must purchase a license if you end up liking the editor and want to use it on a regular basis, but for evaluation the software is free.

"Sublime Text 2 may be downloaded and evaluated for free, however a license must be purchased for continued use. There is currently no enforced time limit for the evaluation." - Sublime Text's license information.

Once you have installed the software on your computer, open it.

## Navigating in Sublime Text

### Package Control

You'll immediately notice that Sublime Text is much simpler than Brackets - but that's OK.  Let's install the *Package Manager* so that you can add some tools to Sublime Text to make it a little more friendly for our class.

Visit the [Package Control installation](https://sublime.wbond.net/installation#st2) website, and copy the code from the "Sublime Text 2" tab.  Now, go back to your Sublime Text editor, and select "View > Show Console" in the menu.  A little window will show up at the bottom of the editor view.  You can paste the code you just copied into this window, and hit enter.  If it worked correctly, the code will run and you will see "Please restart Sublime Text" written in the console window.  Restart Sublime Text.

### Installing a Package

With Sublime Text open, choose "Tools > Command Palette" (or press "cmd+shift+p" on mac).  A window will pop up, allowing you to search all the available commands.  The one we want to use right now is named "Package Control: Install Package".  Start typing and the list will filter, then use your arrow keys or mouse to select "Package Control: Install Package". Hit Enter (or click with your mouse) and the command palette will refresh.  You now have a list of all packages available to install.

Search for the package "SublimeServer".  Click to install it.

### Creating A Project

If you want to see your files in the sidebar like we have in Brackets, you will need to create a project.  In Sublime Text, click "Project > Add folder to project".  Navigate to your project-porfolio folder, and click "Open".

From now on, when you open ST, your project should be open.  If you want, you can save your project, and then it will be able to be opened again if you do want to switch projects.

## Editing and Live Preview

As you are editing files, you can right-click in the code area and choose "Open in Browser".  This opens your file in your default browser (probably Chrome).  To start a local server, like we did with LivePreview, go to "Tools > SublimeServer > Start SublimeServer".  Now, go back and right-click in the code area again.  You'll see a new option for "View in Sublime Server"