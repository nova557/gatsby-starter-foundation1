---
template: blog-post
title: Geography of Typography
slug: type-of-typography
date: 2021-02-14 18:44
description: Typography
featuredImage: /assets/r12be9ed62ac30f5f8a92c4a3ef623281.png
---
<!--StartFragment-->

Typography is making sure that you’re putting letters and text in a certain way that makes it legible and clear to whoever is reading it. It is the CSS Properties that allow you to create the style coding such as the color, size, spacing, and shape of the text. Basic Typography is very important and is a vital component to your overall text. It really does help and provide the overall picture and to make it more personal to your website or blog. It will help the user and guide them to a user friendly way to get information. When letters and words are not spaced right or the right size it makes it difficult to read it. Also, the number of characters you put in each row is also important when text is too long in a line, it makes it harder to read. Here are some basic rules of number of characters you should put in each row:



60 character max: Use this when working with rows of text that are not in columns.

45-50 character max: Use this when putting text in multiple columns.

70-75 character max: Use this when putting text in 1-column.



Here are some other design formulas to keep in mind:



* A font’s point size multiplied by 2 = a columns width (in picas)
* 1 pica = 12 point
* 1 em = the current specific point size.



One example of Typography is Responsive Typography. Responsive Typography styles the font size in your text. You can alter the root font size of the text to make it mid-width or even max-width. It's based on media queries and is the easiest method and has the widest browser support. These methods help on how to create a responsive typography using CSS. It can be used on many devices and/or screen sizes such as mobile, tablet, laptop, desktop, etc. You can use the rem CSS unit to change the size of other typographic elements. For example, an H1 tag with a size of 4.5rem will have a different font size.



| **Viewport Width** | **<640px** | **\>639px** | **\>1023px** | **\>1279px** |
| ------------------ | ---------- | ----------- | ------------ | ------------ |
| Base Font Size     | 16px       | 17px        | 18px         | 19px         |
| H1 Font Size       | 40px       | 42.5px      | 45px         | 47.5px       |
|                    |            |             |              |              |

**\
Write the Coding:**

/\* Define minimum font size \*/

html {

font-size:16px;

}



/\* Define breakpoints and font sizes \*/

@media (min-width:640px) and (max-width:1023px) {

html {

font-size: 17px

}

}



@media (min-width:1024px) and (max-width:1279px) {

html {

font-size: 18px

}

}



/\* Define max font size and viewport \*/

@media (min-width:1280px) {

html {

font-size: 19px

}

}

![]()

Fluid Typography is another example of Typography that is important for Web Development. It is really about how your font size changes depending on your screen size. It is a form of resizing used by viewport units, which are the area of your browser where your content is displayed. To start using Fluid Typography you need to set the font size on HTML. It is a good idea to have a formula in CSS that can update the font size property. The formula for this kind of coding is: min font size + (max font size - min font size) * (100vw - min vw) / (max vw - min vw). The formula would then have the result of:

<!--StartFragment-->



| **Viewport Width**   | **Base Font** |
| -------------------- | ------------- |
|                      | **Size**      |
| <640px               | 16px          |
| 700px                | 16.5167px     |
| 750px                | 16.95px       |
| 1200px               | 20.9px        |
| \>1440px             | 23px          |

<!--EndFragment-->

**Write the coding:**

/\* Define minimum font size \*/

html {

font-size: 16px;

}



/\* Fluid typography formula \*/

@media (min-width: 640px) and (max-width: 1439px) {

font-size: calc(16px + (23 - 16) * (100vw - 640px) / (1439 - 640));

}



/\* Define max font size \*/

@media (min-width: 1440px) {

font-size: 23px;

}



Having these types of Typography that are important to your overall text will help you have easy to read information. It could make your design personal to the reader. It could make it look welcoming or serious depending on how you are laying out your page.



<!--EndFragment-->