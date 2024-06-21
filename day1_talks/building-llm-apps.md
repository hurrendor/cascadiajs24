---
id: lu2lmk78wbv5sqcvk5dmf2e
title: Building LLM Apps
desc: 'Come learn about techniques using LangGraph.js to build with smaller LLMs, and some of the benefits to designing apps to work with OSS models rather than always opting for the largest and most powerful.'
updated: 1718928110916
created: 1718918236008
---
# Building useful apps with small, local LLMs
## Jacob Lee

## Speaker Information
x - (@hacabu)[https://twitter.com/hacubu]
@LangChainAI
smith.langchain.com
(Tutorials)[https://langchain-ai.github.io/langgraphjs/tutorials]
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/building-useful-apps-with-small-local-llms]

## Why Small Language Models?
Bigger is sometimes better but..

### Smaller Models have Portability 
Examplese - webml-demo.vercel.app, webllm.mlc.ai, ollama.ai

### Better design = better reliability
Smaller models force you to think about what you're doing

### Current LLM landscape
Timelinei provided to show rapid progression in LLMs from June 2017 to June 2024.

## How do you build with the future in mind?
Focus on productionization and architecting well, it's too early to "build for" a specific model.

(Chatbot arena leaderboard)[https://huggingface.co/spaces/lmsys/chatbot-arena-leaderboard]
Consider how many resources are needed to use the chat bot.


## Levels of Language Model
Human driven models <-----> Agent Executed
1. Code
2. LLM Call
3. Chain with multiple LLM calls
4. Router
5. State Machine
6. Agent

### Using LangGraph
LangGraph thinks of flow states as nodes.
- Customize a cognitive architecture
- Optionally use LangChain modules
State is central 
    - checkpoints for rewinding and debugging
    - allows for interruptions or human intervention in the loop
LangSmith for productionization

Designing out a small model with RAG and Self Reflection
Ask a question, retrieve a node and grade the node. Create a process flow that checks for hallucinations, relevant docs, and if the question asked is actually answered.