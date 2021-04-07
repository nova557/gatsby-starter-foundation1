---
template: blog-post
title: PS CSS Animations Are Great!
slug: css-animations
date: 2021-04-04 16:58
description: CSS Animations
featuredImage: /assets/rb642b5918e026cbb688c0fa3759a5cb9.jpg
---
<!--StartFragment-->

Everyone has their own way of coding something. They use different tools, different resources, and have their own ideas on what they want to create. I have found that CSS Animations can be a great way to do just that and can help learn to do better with your coding.



CSS Animations can be many things and has many properties that you can use with it. Here is an example of an animation:

**<!-- HTML -->**

**<div class="simple-spinner"></div>**



**/\* CSS \*/**

**.simple-spinner {**

**height: 48px;**

**width: 48px;**

**border: 5px solid rgba(150, 150, 150, 0.2);**

**border-radius: 50%;**

**border-top-color: rgb(150, 150, 150);**

**animation: rotate 1s 0s infinite ease-in-out alternate;**

**}**

**@keyframes rotate {**

**0% { transform: rotate(0); }**

**100% { transform: rotate(360deg); }**

**}**

![](/assets/simple-spinner.gif "Simple Spinner")

This coding is to make an Animation using HTML and CSS. The animation that it creates is a loading circle that rotates when you write the coding. It is an animation because it creates an object that rotates just as in the coding. First thing you have to do is build a ring with a <div> tag that has the same width and height. Then, make a border where one side has a different color, while having a border radius of 50%. Lastly, to make the animation work you have to make the animation property for the element that you want to animate and create a @keyframes rule.



The Animation Property can be a number of different properties from your choosing at once. Examples are; animation-name, you can name the animation whatever you want; animation-duration, how long that you want the movement of the animation to last; animation-delay, how long to wait before you want the animation to start; animation-iteration-count, how many times you want the animation to be repeated; animation-timing-function, how an animation progresses in one cycle; animation-direction, where you want the animation to move from (forwards, backwards, back and forth). These are some of the properties that were used for the simple spinner animation above.



The @keyframes rule is a big part for creating the animation. You can change when to appear (a percentage of the animation time) and which styles you want to add to it. There are many things that you can put under @keyframes that creates the animation. For example, 0% transform: rotate(0) gives you no rotation for the spinner animation, while 100% transform: rotate(360deg) gives you a full rotation. It can be used by multiple elements. Here is another example of a different animation:

**<!-- HTML -->**

**<div class="double-spinner"></div>**



**/\* CSS \*/**

**.double-spinner {**

**height: 48px;**

**width: 48px;**

**border: 5px solid rgba(150, 150, 150, 0.2);**

**border-radius: 50%;**

**border-top-color: rgb(150, 150, 150);**

**animation: rotate 1s 0s infinite linear normal;**

**}**

**.double-spinner::after {**

**content: '';**

**height: 40%;**

**width: 40%;**

**display: block;**

**margin: 10px auto;**

**border: inherit;**

**border-radius: inherit;**

**border-top-color: inherit;**

**animation: rotate .5s 0s infinite linear reverse;**

**}**

**@keyframes rotate {**

**0% { transform: rotate(0); }**

**100% { transform: rotate(360deg); }**

**}**

![](/assets/double-spinner.gif "Double Spinner")

It is true that you can create multiple animations to the same element. If you want to make your animation flip, move, glow, or more all in the same shape at the same time, you can add another animation separated by comma. For example:

**/\* CSS \*/**

**.flip-walker::before {**

**/\* ... \*/**

**animation:**

**flip 2s 0s infinite ease normal,**

**glow 2s 0s infinite linear normal;**

**}**

**@keyframes flip {**

**/\* ... \*/**

**}**

**@keyframes glow {**

**to { background: white; box-shadow: 0 0 15px white; }**

**}**

![](/assets/flip-walker-before.gif "Flip Walker")

This will create an animation of a square inside a big square glowing and moving around in the shape of a square. It looks pretty cool when you finish it.



The Custom Timing Function is another aspect for CSS Animations. After you create the animation that you want and are not happy with the Default Timing Functions, you can use a certain tool such as a cubic-bezier-curve. Here is an example of what you have to change in the coding:

**<!-- HTML -->**

**<div class="pulse"></div>**



**/\* CSS \*/**

**.pulse {**

**width: 64px;**

**height: 64px;**

**background: white;**

**border-radius: 50%;**

**animation: pulse 1s 0s infinite cubic-bezier(0.000, 1.010, 0.5, 1.200) normal;**

**}**

**@keyframes pulse {**

**from { transform: scale(0); opacity: 1; }**

**to { transform: scale(1.0); opacity: 0; }**

**}**

![](/assets/pulse.gif "Pulse")

**All you have to do is replace the timing function to cubic-bezier(0.000, 1.010, 0.5, 1.200).**



Fallbacks is another useful tool for CSS Animations. If you want to support older browsers in your animation, then you can use the @supports at-rule for a feature query and can provide a Fallback e.g. as a GIF. Here is an example:

**/\* CSS \*/**

**.animated {**

**background: url(animation-as.gif);**

**}**

**@supports (animation-name: test) {**

**.animated {**

**background: none;**

**animation-name: test;**

**/\* ... \*/**

**}**

**@keyframes test {**

**/\* ... \*/**

**}**

**}**

Browsers that don't support the animation-name property or even the @supports rule will simply show the GIF image as the background of your element.



I feel that CSS Animations is a great start for people who are beginning to learn about it. It is a great way for entertaining people and to entertain the people who create it. I am sure that after you keep coding animations and adding more and more properties and tools to it, you could make something that is really spectacular.



<!--EndFragment-->