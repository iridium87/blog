---
layout: post
title: "How I Explain an LLM to Myself"
date: 2026-05-04 10:00:00 +0100
categories: [AI, LLM, notes]
---

After working a bit with LLMs I started to look for a way to explain them to myself and how they work, but also try to find an explanation that will land with my colleagues, family and friends. This is what I got.

An LLM is at its heart a complicated statistical machine, which gives a statistically significant answer based on the data it was trained on and based on the data you provide it. The answer is not right or wrong, it is statistically significant or "likely" based on the training data and the data you provided. As opposed to common knowledge, an LLM actually never hallucinates, there is no such thing! If you do not give it data to work on, the model will use its training data to again give you a statistically significant answer. So, in its world it is never wrong and technically it isn't — it just gave you an answer for someone else.

Whether statistically significant is good enough for you is up to you. 60% could be okay in some case, say writing a mail to a colleague. In others, 90% statistically significant is not good enough.

The other important thing to realize is that there is actually not "chat" with an LLM — this is just an illusion built to help the experience. What an LLM does is complete sentences based on what you provided and the training data of the model, like so:

```
A dog is chasing a... complete the sentence


A dog is chasing a fox
```


Training data, statistically valid, generally true.


Now comes the tricky part:

```
Can YOUR dog catch THIS fox, today, in THIS garden
```

Specific, contextual, requires real data about your actual dog and your actual fox.

I think it is important to understand how LLMs work so you can control them, know what to expect, understand when they fail and most importantly — why they fail. It is just another tool at the end of the day.
