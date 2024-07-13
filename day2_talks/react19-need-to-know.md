---
id: 6ppubd6b0b0wv0jxoecv1ci
title: React19 Need to Know
desc: 'React 19 Beta is here! This new release brings a suite of exciting updates. From new hooks and Actions to changing the way we use refs, React 19 is going to change how we build web applications and use hooks. In this deep dive talk, we will explore the new features of React 19. Learn everything you need to know about Form Actions, the React Compiler, and new hooks such as useOptimistic and useFormActions. Additionally, we will delve into the capabilities of React Server Components.'
updated: 1718991052315
created: 1718990986332
---
# Everything You Need to Know About React 19
## Shruti Kapoor

### Speaker Information
x, Twitter, YouTube - (@shrutikapoor08)[https://twitter.com/shrutikapoor08]
Website - (shrutikapoor.dev)[https://shrutikapoor.dev/]
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/everything-you-need-to-know-about-react-19]


## React 19 RC - Release Candidate

### React Actions
enable easier form handling
`startTransition()` ('react18') shows most urgent changes

### React Compiler
removes the need for `useMemo`, `useCallback` by providing auto memoization in/on hooks and components.
Produces re-renders by skipping re-rendering of children when the parent updates
Skips expensive calculations by identifying expensive React hooks.
Functions within components are also auto memoized, but not functions outside of Components


### New Hooks
(useFormStatus) - gives info of the last form submission. 
`useFormStatus()` - provide `pending`, `data`, `method`, `action`
Attributes need to be used inside of the form / in a child component

`useActionState()` - Identify a form action for handling the form submission.
The hook takes an action
ex` - <form action={formAction}>`

`useOptimistic()` 

### New APIs
`use` - doesn't follow the rules of hooks; can be anywhere in the component
Can only be used in render

### Changes
- `ref` is a now a prop - no more `forwardRef`
- Removing `useMemo`, `useCallback`
- Accepting prioritizing of stylesheets and when they load