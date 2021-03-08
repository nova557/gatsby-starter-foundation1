---
template: blog-post
title: Responsible Responsive Layouts
slug: responsive-layouts
date: 2021-03-07 19:59
description: Responsive Layouts
featuredImage: /assets/responsive-design-illustration.jpg
---
<!--StartFragment-->

Accommodating all devices for users is the best way to go when making any Interface design. The way you put the information in with coding is so important. You do not want to leave any one user behind. I have found that using a responsive layout works well.



Responsive Layouts is a type of coding that can be used for HTML and CSS. While using it on a website you can resize, hide, shrink, or enlarge it to make it look good on the site. It can be used on any device such as; desktops, tablets, and phones. Some Responsive Layouts include; Viewport, Dependant Sizes, Columns and Flowing, Expanding coverage, Collapsing and Hiding, Rearrangement, and Altogether.



The viewport is the view of the page that can be any size from being the view of an Ipad, Iphone, or Laptop. You can add a viewport to the page which tells the browser how to control the page’s dimensions and scaling. The coding is:

<meta name="viewport" content="width=device-width, initial-scale=1.0">



![See the source image](https://lh6.googleusercontent.com/S6CCWcLEfGT9XvZDwlCJcXbjBZYuO3XCTc569xxvLtJSBg1NUxcskTTmxy8aSGIQ8QgpvpwH8Wq33p0orB7a00wT04BuIW3LsLH_a58nb6eCQdEZmMe2D3P3QWh2--7xI-kCwUZ2)

As you can see in the picture above how important it is to have the right layout on your design. Using this meta tag really makes a difference in the way that you view the page especially if you are viewing on a phone or small tablet. It is vital to be able to read even the small parts of the text that describe the page's layout. Meta tags always go inside the head element and are mostly used to describe the page.

To create a Meta Tag:

1. Adjust the title in the source - HTML Title tag. Click on the first phrase you will see as a result in the search engines is the title.
2. Add a relevant description - meta description tag.
3. Make sure your page works on mobile devices.
4. Put it all together.



Another Responsive Layout you can use involves adjusting the Columns and Flowing on the page. On any device such as a phone, in portrait layout, you can view several items listed vertically. While on the other hand, a tablet has more space to have columns and to view more items. The items flow into the columns and fill the columns left to right and hit the end of the row wrap to the next one. Many websites have a Responsive Layout with 1-3 Fluid columns using Grid Template areas. This type of website has content sidebars, a header, and a footer. You may want to use the Layout as a single column in a Responsive Design, then you can add a sidebar and then use a three column layout for wider screens.

![Image of the three different layouts created by redefining our grid at two breakpoints.](https://lh6.googleusercontent.com/DR3Xu-vZReBJhFwUKmABahDVwKKCqSRPLaKk5y9PcweH2KWe5ZdZxO89iw2-ucy6MXQZRPQ0NVN4bCC6jk9PTA_7o_qTbtrV545tP4KRpOLrKGanauwaESSDENZ8O3SKhg1GCkt1)

Here is an example coding Grid Template Areas:

<div class="wrapper">

<header class="main-head">The header</header>

<nav class="main-nav">

<ul>

<li><a href="">Nav 1</a></li>

<li><a href="">Nav 2</a></li>

<li><a href="">Nav 3</a></li>

</ul>

</nav>

<article class="content">

<h1>Main article area</h1>

<p>In this layout, we display the areas in source order for any screen less than 500 pixels wide. We go to a two column layout, and then to a three column layout by redefining the grid, and the placement of items on the grid.</p>

</article>

<aside class="side">Sidebar</aside>

<div class="ad">Advertising</div>

<footer class="main-footer">The footer</footer>

</div>

Here is another example of coding the Grid Template Areas:

.main-head {

grid-area: header;

}

.content {

grid-area: content;

}

.main-nav {

grid-area: nav;

}

.side {

grid-area: sidebar;

}

.ad {

grid-area: ad;

}

.main-footer {

grid-area: footer;

}

Dependent SIzes are a crucial layout that is important for coding. For example, a Title Bar. Coding: Panel {Padding=5,2,5,4}

Icon {Alignment=Left Type=Menu}

Icon {Alignment=Right Type=Share}

Text {Alignment=Center Value="News Browser"}

Rectangle {Alignment=Bottom Color=Black Height="2"}

This will create a Responsive Title Bar. It will take up the whole width, the icons positioned at the sides, and a dividing line no matter what device you are using. The dependent sizing provides features that can be really useful for Responsive Layout.



Flexible Grids are a way to not have to worry about accommodating every device that is in the world today but it definitely gives you a better way to change what looks bad from the breakpoint.

Here is an example of how to make a responsive design using media queries and a Flexible Grid.

![A mobile view of the layout with boxes stacked on top of each other vertically.](https://lh5.googleusercontent.com/L3NcPctQD1DcW317e2oae2nWTnnJqdANXiT7IaVqGH3_XuUKyti8L8twjsGjYS0r9NLBnReB2FUkzX6EdwRFEWi0R-NKsO52UEwCxp4D09l9CXbvXqw_Q30aQ-CTmdMxnJ5U3mqQ)

On wider screens they move to two columns:

![A desktop view of a layout with two columns.](https://lh3.googleusercontent.com/K6f7MTt1M5LZRAP2QVd3sZMSTtrQfsv3dLbC54p-THQlozvKIsx4ySkwvMStSMwuRF6V5woK9FnDLIG06Qr_MBeOS0aS5O0MW1zsiRt5Nc0ejDbdfnJe8viTLsgMi34u2Nef_6Lt)



There are 3 modern layout ways that you can create a Flexible Grid. The first one is Multicol. Multicol is a layout method that when you write in column-count it shows you how many columns that you want your content to have. The browser will then change according to screen size.

.container {

column-count: 3;

}

This is the code for column width:

.container {

column-width: 10em;

}



The second Modern Layout is Flexbox. In Flexbox, you can change the size of the items using the code Flex-Grow or Flex-Shrink. It will give you space between the items. Below is an example of the Flex item with an equal amount of space using the code:

.container {

display: flex;

}

.item {

flex: 1;

}

The last Modern Layout is the CSS Grid Layout. This coding will determine how you position your items on the page. With the fr unit coding it helps you get available space in your picture. Here is an example of the Flexible Grids Coding with the fr unit:

.container {

display: grid;

grid-template-columns: 1fr 1fr 1fr;

}

These Responsive Layouts are all very useful for your coding. You want to make a good design, then these Steps will help you greatly.



<!--EndFragment-->