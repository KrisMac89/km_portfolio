---
layout: post
title:  Jekyll Theme Tutorial
date:   2018-07-30 05:55:01 -0400
categories: jekyll update
permalink: theme tutorial
---
Jekyll is an agile static site generator designed to speed up the building process. It provides some neat features to aid content creation. For an introduction to the framework visit the <a href="https://jekyllrb.com/docs/home/" target="\_blank">Jekyll website</a>. Today we will be talking about Jekyll's gem-based themes. Themes are site templates created by the community that can be implemented to style your site.

Themes are varied; some may simply provide a background and alter how your posts and pages are displayed. Others may overhaul every aspect of a typical website down to the form tags you never intended to use. By default, Jekyll sites come installed with the minima theme. You can begin perusing different themes by navigating to <a href="https://rubygems.org" target="\_blank">rubygems.org</a> and searching jekyll-theme.

<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/rubygems.jpg">

(Note: There are plenty of sites for jekyll themes, rubygems.org just happens to have lots of them and sorts by  most popular!)
<br />

Select any theme, choose Documentation from the Links section, and search for a theme preview link in the theme's README file. The preview, while not always included, can provide a browser's glimpse of the site layout. The README file will describe different features of the theme whether or not a preview is provided. Explore your theme's GitHub repository as well to better understand its directory and the typical hierarchy seen in Jekyll themes.

<br />
<h1>Installation</h1>
Once you have selected your theme it's time to install it! Locate the name of your theme (top) which can be found on its GitHub repository and add it to your site's Gemfile (bottom):

<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/themename.jpg">
<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/gemfile.jpg">
<br />

Now run this command in your command prompt under your site directory to install the theme:

<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/bundleinstall.jpg">
<br />

Specify the theme in our config.yml file:

<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/themeinyml.jpg">
<br />

Lastly, we run our Jekyll server and allow it to configure the theme:

<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/bundleexec.jpg">
<br />

Now our site should start using our new Jekyll theme. The only issues we may run into are the default site's front matter. The minima theme has a post, page, and home layout. Many of the themes that you come across will have their own layouts or may simply have a default layout for the site. Make sure to edit your yml front matter on your pages and posts to reflect the layouts in your theme.

<br />
<h1>Customization</h1>

Themes are a fast way to build a clean website but there will be times when the creator wants to edit the theme's style to suit their needs. To do this we must make a copy of the theme file that we wish to edit and place it in a correlating directory in our site.

For example: index.md (the home page) specifies "layout: default" in its front matter. In order to edit the design of index.md we will have to create a directory called \_layouts and, either copy/paste the theme's default.html file into this directory, or create a new file under this directory called default.html and style it from scratch.

When your site uses a theme, it searches in your directory for referenced files like \_layouts and \_includes before searching the theme's directory. We can customize themes using this logic to our advantage by overriding theme files with our own. Discover your theme's file path on your PC by running the following command, replacing the theme name accordingly. By mirroring your theme directory you can replace any file you wish to edit:

<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/showtheme.jpg">
<br />

You can also copy/paste all your theme directories into your site directory and remove the theme name from your yml file to stop receiving updates to your theme. Experiment with different site templates and overriding their features to suit your site's needs. At this point, you should be able to install and customize gem-based themes for Jekyll to create fully styled blog sites very quickly.
<br />
<br />
<img src="https://krismac89.github.io/km_portfolio/assets/images/jekyll.png" width="300" height="110">
