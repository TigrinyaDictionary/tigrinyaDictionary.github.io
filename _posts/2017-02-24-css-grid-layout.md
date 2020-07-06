---
layout: post
title: CSS GRID LAYOUT
description: Elements can be placed in grid like structure using CSS, css grid style, web site developer
---


* CSS grid layout display contents in two dimension. Elements can be placed in grid like structure using CSS.
* CSS grid layout defines rows and columns.
* CSS grid layout can be changed based on media queries, making responsive design easier.
* CSS grid layout for overlapping items in grid. The order of items can be controlled using z-index.


<h4 class="te-header"> An example of required layout for desktop,tablet and mobile devices: </h4>
The required layout for desktop and mobile devices can be easily achieved using grid css. Steps to achieve the layout will be:

* Declaring the grid
* Placing items

![ALT Grid style for desktop](/assets/Images/Blogs/Css-grid-style/desiredlayout.png)


<script async src="//jsfiddle.net/Kiflay/Lsxkcvne/3/embed/html,css,result/dark/"></script>

<h4 class="te-header"> Declaring the grid: </h4>

We declare a grid with 3 rows and 3 columns. The first, third rows and columns  are sized to fit the content. The second row and column takes up the remaining size.  

![Declare the grid](/assets/Images/Blogs/Css-grid-style/declareGrid.png)
 
<h4 class="te-header"> Placing Items: </h4>
We have placed grid items using the ‘grid-area’ shorthand. For example the side panel items is placed on grid area “sidePanel”
 
![placing items](/assets/Images/Blogs/Css-grid-style/placingItems.png)





