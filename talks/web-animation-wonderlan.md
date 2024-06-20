---
id: 0gdg4kkkr2r3jpmgy335soe
title: Web Animation Wonderland
desc: 'Ages ago, when CSS animations were young and the Web Animations API had yet to ship in all browsers, before the time of JavaScript frameworks when JQuery could still be found on job postings, Rachel Nabors made a series of interactive, hand drawn Alice in Wonderland storybooks using polyfills and some clever hacks. Today, jump down the rabbit hole again with brand new CSS and Web APIs that bring your wildest dreams to life. Join Alice, Rachel, and the Hipster White Rabbit as they refactor Alice in Web Animation Land.'
updated: 1718900170967
created: 1718900136459
---


# Return to Web Animation Wonderland
## Rachel Lee Nabors
(Recorded Talk)[TBA]


### Speaker Information
x - @rachelnabors
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/return-to-web-animation-wonderland]

WebAnimations API
js/tunnel-animation.js

## General Animations
Replacing previous CSS linear animations by using the JS built-in WebAnimations API!
Notable classes:
Animation
KeyframeAnimation
Animation classes come with play, pause, stop methods.
Use specialty classes 

## Scroll-driven animations
Identifying the when - timelines, and
the what - /** missing **/ 
ScrollTimeline

CSS5 - version

## View-driven animations
Using the ViewTimeline class

Just CSS5 - use animation-timeline

## Chaining animations
### fScroll Timeline vs View Timeline


## CSS5 MPA View transitions
Limits: only works in browsers running Chromium 126+
(Polyfills for Safari/Firefox)[github.com/flackr/scroll-timeline]
Scroll-Driven Animations Debugger - Chrome Extension

`` @view-transition { navigation: auto } ``
Unsupported browsers just show a regular page swap.