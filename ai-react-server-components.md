---
id: 5wksmr0vmr1274nsy9ll3xv
title: Ai React Server Components
desc: 'In this talk, we'll explore how we can use powerful techniques to generate React Server Components and then use them on the client to relay rich information to our users, providing the best possible user experience.'
updated: 1718929654685
created: 1718918377386
---
# AI-Generated React Server Components
## Tejas Kumar

## Speaker Information
x - [@tejasKumar_](https://twitter.com/tejasKumar_)
Website - https://tej.as
Youtube @tejask
(Cascadia Talk Information)[https://cascadiajs.com/2024/talks/ai-generated-react-server-components]

## AI
3 Types of AI:
- Rule-based

- Predictive
Roots around early 1900's using the Markhov chain of predicting the next results. There is no memory around the predictions given, it only works off of a current value it's parsing.
Google Paper - (Attention is All You Need)[https://research.google/pubs/attention-is-all-you-need/]

- Generative
GenAI

Problems with GenAI
- Hallucinations
- Finite context length
    Context is lost after longer periods of content. 
- Knowledge cutofff
No real time information is given.
- LLMs produce mostly text

## RAG - Retrieval Augmented Generation
Retrieve data, augment the generated text

## RAG components
- Data

- Embeddings models
Turns requests into an fixed length array. Vector search is used to identify answers in the same proximity of what is being looked for. 
- Vector store

LangFlow can be used to map questions to the different nodes and vectors and start bringing in real time data

## Generative UI - Live code demo
Utilize a tools attribute from an AI LLM library to be able to provide React components back to the user.