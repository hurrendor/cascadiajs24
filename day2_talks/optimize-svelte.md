---
id: ymllyxuctjjz0ya771dxwa7
title: Optimize Svelte
desc: 'Let's look at what's new in Svelte 5 and how it makes Svelte apps more performant, more scalable, and easier to reason about. We'll also unpack why the changes were made and how they were rolled out.'
updated: 1718918858723
created: 1718918802246
---
# Optimize for vibes: Svelte 5 and the new age of Svelte
## Geoff Rich
[YouTube Recording](https://www.youtube.com/watch?v=PQluuawldDE&list=PLLiioAbFTbKPi9SkDhtppEGDPI31GGZyj&index=13&pp=iAQB)

## Speaker Information
x - (@geoffrich_)[https://twitter.com/geoffrich_]
(Slides)[TBD]
(Website)[https://geoffrich.net]
(cascadia Talk Information)[https://cascadiajs.com/2024/talks/optimize-for-vibes-svelte-5-and-the-new-age-of-svelte]

## Resources:
(Svelte 5 Preview Docs)[https://svelte-5-preview.vercel.app/docs/introduction]




## What is Svelte
"A compiled, batteries-included, HTML-first JavaScript framework that prioritizes vibes"

### Compiled
Svelte uses compiler first and compiler only

### Batteries included
Includes accesibility flags and other features built in.

### HTML-first
Svelte builds on using HTML first and adding JavaScript activity

### prioritizes vibes
Svelte focuses on how it feels to write with it. The project with a change should still feel the same to work with after adding a change.

### Svelte breakdown
`$` defines a reactive block that automatically updates on the UI when the value changes.

## Svelte 5
Main goal for Svelte 5: universal runtime reactivity

### Runes
Svelte 5 will use `runes` to provide an order to the Svelte compiler to run a function.
ex: `$state(0)`, `$effect()`
Uses getters for property values
```
    let count = $state(0)
    get count() { return count }
``` 
### State
State is now explicit rather than assuming every `let` statement is a state setup.

### Effect
Determines when to re-run based on the values changing
ex `$: { console.log(count)}`

### Signals
Holds a value, and tracks when that value is read (dependencies)
Will trigger updates in used locations when the value is updated

### Scaling
Larger runtime, smaller component size. Larger apps will make better use of the smaller components.
