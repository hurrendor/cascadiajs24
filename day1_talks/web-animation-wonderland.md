---
id: 0gdg4kkkr2r3jpmgy335soe
title: Web Animation Wonderland
desc: 'Ages ago, when CSS animations were young and the Web Animations API had yet to ship in all browsers, before the time of JavaScript frameworks when JQuery could still be found on job postings, Rachel Nabors made a series of interactive, hand drawn Alice in Wonderland storybooks using polyfills and some clever hacks. Today, jump down the rabbit hole again with brand new CSS and Web APIs that bring your wildest dreams to life. Join Alice, Rachel, and the Hipster White Rabbit as they refactor Alice in Web Animation Land.'
updated: 1718900170967
created: 1718900136459
---
# Return to Web Animation Wonderland
## Rachel Lee Nabors
[YouTube Recording](https://www.youtube.com/watch?v=CtLbO0UCYLc)
[Slides](https://www.dropbox.com/s/umtanfexdkh48dz/Alice%20Returns%20to%20Web%20Animations%20API%20Land%20slides.pdf?dl=0]
(Resources)[https://github.com/rachelnabors/alice-in-videoland)


## Speaker Information
- x - @rachelnabors
- Substack - [nearestnabors.substack.com](nearestnabors.substack.com)
- Website - [nearestnabors.com](nearestnabors.com)
- [Cascadia Talk Information](https://cascadiajs.com/2024/talks/return-to-web-animation-wonderland)

WebAnimations API
js/tunnel-animation.js

## General Animations
Replacing previous CSS linear animations by using the JS built-in WebAnimations API!
Notable classes:
- `Animation`
- `KeyframeAnimation`
Animation classes come with play, pause, stop methods.
Use specialty classes 

## Scroll-driven animations
Identifying the "when" -> timelines
the what -> /** TODO: Fill me in with missing data! **/ 
ScrollTimeline

CSS5 - version

## View-driven animations
Using the ViewTimeline class

Just CSS5 - use animation-timeline

## Chaining animations
### Scroll Timeline vs View Timeline


## CSS5 MPA View transitions
Limits: only works in browsers running Chromium 126+
[Polyfills for Safari/Firefox](github.com/flackr/scroll-timeline)
Scroll-Driven Animations Debugger - Chrome Extension

`` @view-transition { navigation: auto } ``
Unsupported browsers just show a regular page swap.