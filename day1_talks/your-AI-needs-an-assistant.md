---
id: 006umib0lp015rtpjenir3p
title: your-AI-needs-an-assistant
desc: 'AI can write lots of code - just, not always good code 😬. Let's see how our existing tests and tools can work alongside new AI fanciness to make the most productive dev cycles we've ever seen. 🚀'
updated: 1718903029220
created: 1718902964771
---
# Your AI Needs an Assistant
## Josh Goldberg

### Speaker Information
x - (@)[]
Twitch - @
Website - JoshuaKGoldberg
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/your-ai-needs-an-assistant]


The rise of AI has led to unconventional usage of different tools.

## The Gartner Hype Cycle
- Peak of Inflated Expectations
- Trough of Disillusionment
- Plateau of Productivity

LLM 'AI' is just globally aware autocomplete. 'AI' is a tool, not a feature.

## Plan of Attack
1. Documentation
Please, read the docs first. Understand the tool. AI just regurgitates information it's given.
2. Static Analysis
Formatters, linters, and type checkers (ie TypeScript)
AI returns formatted code that could benefit from linting and type checking.
3. Dynamic Analysis - Testing!
Give your AI prompts as much context as possible.
Tools: Sourcegraph - Cody, LangChain
4. Dynamic Static Analysis - Running static analysis, dynamically
Give the AI data shapes that you expect to work with.
Tool - (github.com/Microsoft/TypeChat)[https://github.com/Microsoft/TypeChat]
Use tools like TypeChat to 
5. Dynamic Dynamic Analysis - Running dynamic and static analysis, dynamically
AIs are good at ideation,
Dev tools are good at verification!
Combine the two systems for a better product.
(Code Example using Gemini)[https://github.com/JoshuaKGoldberg/gemini-codegen-example]

Predictions for the Future
Codegen will use AI in conjunction with existing dev tools. We'll see faster, specialized AI for specific tasks.