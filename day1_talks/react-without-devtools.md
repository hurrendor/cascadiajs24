---
id: ttxly03uxtdnkjzuztn0gv2
title: React without Devtools
desc: 'React DevTools today help find slow components in your React app. But Devtools are complicated to use: we insert profile everything, catch some promising leads, but nothing happens before time runs out. Eventually, the slow/buggy code never gets fixed, problems pile up on a backlog, and our end users are hurt.

But what if we could find these issues... automatically? In this talk we’ll discover Million Lint, and how we can use compilers that let you do exactly that.'
updated: 1718903409017
created: 1718903289910
---
# React Without DevTools
## Aiden Bai
[YouTube Recording](https://www.youtube.com/watch?v=_iqhkmPfOEQ)

## Speaker Information
- x - (@aidenybai)[https://twitter.com/aidenybai]
- [Website](million.dev)
- Company - millionJS
- [Cascadia Talk Information](https://cascadiajs.com/2024/talks/react-without-devtools)

## Performance optimization investigation
Options like devtools, `useMemo` hook, react compiler all provide options but no insights into the performance.
Decoupling performance data from the code makes it difficult to understand.

Callback functions are recreated every rendering.
Separate the input value from the filter value.

Recommending: Million Lint to provide code optimization and linting capabilities.