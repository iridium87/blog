---
layout: post
title: "Quantization in llama.cpp"
date: 2026-05-11 10:00:00 +0100
categories: [AI, LLM, technical]
---

A model has its weights, which can be quantized and embedded in the GGUF file, helping reduce the file size which needs to be loaded in VRAM. This process can be done by llama.cpp as well, but it is an offline process and usually worse than actually downloading a fine-tuned and tested quantization.

What is maybe less known is that the KV cache can also be quantized! There are llama.cpp flags allowing for it, which can save a huge chunk of memory without major degradation. This is where TurboQuant or RotorQuant aim to optimize further.

Another even less known quantization is for the speculative drafter KV cache *(yes, a speculative drafter has its own cache)*, which can further reduce memory use.

---

<p style="text-align:center">∎</p>
