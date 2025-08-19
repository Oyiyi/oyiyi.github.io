---
title: "Exploring the Limits of Fine-Tuning in Language Adaptation for Large Language Models"
collection: publications
category: manuscripts
permalink: /publication/2024-04-files-Exploring-the-Limits-of-Fine-Tuning-in-Language-Adaptation-for-Large
excerpt: 'We were among the earliest to fine-tune LLaMA 3 for multilingual question answering (Q&A) tasks. In this work, we adapt English-pretrained LLMs to Chinese and Turkish Q&A through Parameter-Efficient Fine-Tuning (PEFT) techniques such as LoRA and QLoRA. <br/><br/>Our method enables memory-efficient training on just two NVIDIA 3090 GPUs, showcasing effective cross-lingual transfer with constrained hardware resources.'
date: 2024-04-30
# slidesurl: 'http://oyiyi.github.io/files/slides1.pdf'
paperurl: 'http://oyiyi.github.io/files/Exploring the Limits of Fine-Tuning in Language Adaptation for Large.pdf'
arxivurl: 'https://arxiv.org/abs/2505.20650'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
The emergence of Large Language Models over the past few years has enabled new applications of natural language tasks, specifically in the field of language adaptation. It is computationally expensive to train new Large Language Models from scratch due to the billions of parameters in these state of the art models and the scale of training data.

From our inference trials, the newly launched Meta-Llama-3-8B-Instruct (April, 2024) doesn’t do well in conversations in languages other than English. In this work, we present a method to fine-tune different base models trained primarily on English text to adapt the model for Q&A for the Chinese and Turkish language.

The objective was to create custom foreign language agents from the base model using fine-tuning. Full fine-tuning was not an option as it requires significant resources, so we solved to use Parameter efficient fine tuning (PEFT). In PEFT, we further evaluated two approaches namely LoRA and QLoRA. In both of these approaches we take pretrained weights and freeze them. Then we inject trainable rank decomposition matrices in each layer of the transformer. QLoRA does another optimization on top of LoRa which further reduces the memory footprint. It does a recoverable quantization of model parameters in 4 bits. We used two 3090 GPUs in this workstream.