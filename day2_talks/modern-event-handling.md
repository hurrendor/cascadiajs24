---
id: m135d8y8bprkj3jzph839fy
title: Modern Event Handling
desc: 'Sick of nested and clunky addEventListener() calls? Want a functional, declarative way of handling events in JavaScript? Chrome engineer Dominic Farolino introduces the long-awaited Observable API, a composable event handling primitive to replace addEventListener() coming to a browser near you!

Native Observables do for streams of events what Promises did for callbacks & callback hell. Frameworks have long used them to declaratively create pipelines of operators through which events flow, and the Web is finally getting them natively. Observable API is the most wanted web standards proposal on GitHub by developers, and in this talk you'll learn how to listen to events with an Observable, use operators to transform & listen to multiple events, and even build your own Observables from scratch!'
updated: 1718918776145
created: 1718918706035
---
# Modern Event Handling: A Peek at the New Observable API
## Dominic Farolino
[YouTube Recording](https://www.youtube.com/watch?v=AUYAfayMUl0&list=PLLiioAbFTbKPi9SkDhtppEGDPI31GGZyj&index=12&pp=iAQB)

## Speaker Information
x - [@domfarolino](https://twitter.com/domfarolino)
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/modern-event-handling-a-peek-at-the-new-observable-api]

Github(github.com/domfarolino)[https://github.com/domfarolino]
[Chromium repository for the Observable API](https://github.com/WICG/observable)
Chrome flag to use the Observable API - chrome://flags/#observable-api

## History of `async` on the Web
### 1. Promises & Callbacks
Callbacks provide a non-lineara control flow because of how they break up the functionality. This is somewhat controlled with `.then` chaining.
#### Promise Limitations
For use in events, by the time that the promise returns, the value may not be as ueeful.
## 2. Observables Save the Day
Observables are "promises for multiple values".
Handling a stream of async events, the stream can be manipulated with operators.
Intention is to work with eventTarget better.

## 3. Observables in Action
Both promises and observables have producer & consumer code
Main differnece is that promises are eager and run right away, sometimes before there's a consumer.
Observables are lazy, take many values, and can be subscribed to at any time. Observables are also synchronous.

## 4. Observable Operators (methods)
Derived from JavaScripts TC39 Iterator helper docs.
`.take(int)` can be used to limit the values returned and handled

## 5. Unsubscription and teardown
Terminating operators like `take`, `takeUntil` and `first` use signals that signify when to tear down the subscription.