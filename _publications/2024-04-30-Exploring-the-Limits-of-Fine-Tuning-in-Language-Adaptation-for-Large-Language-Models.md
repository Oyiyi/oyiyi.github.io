---
title: "Exploring the Limits of Fine-Tuning in Language Adaptation for Large Language Models"
collection: publications
category: manuscripts
permalink: /publication/2024-04-30-Exploring-the-Limits-of-Fine-Tuning-in-Language-Adaptation-for-Large-Language-Models
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2024-04-30
# venue: 'Journal 1'
paperurl: 'http://oyiyi.github.io/files/Exploring the Limits of Fine-Tuning in Language Adaptation for Large Language Models.pdf'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
The emergence of Large Language Models over the past few years has enabled new applications of natural language tasks, specifically in the field of language adaptation. It is computationally expensive to train new Large Language Models from scratch due to the billions of parameters in these state of the art models and the scale of training data. 

From our inference trials, the newly launched Meta-Llama-3-8B-Instruct (April, 2024) doesn’t do well in conversations in languages other than English. In this work, we present a method to fine-tune different base models trained primarily on English text to adapt the model for Q&A for the Chinese and Turkish language.

The objective was to create custom foreign language agents from the base model using fine-tuning. Full fine-tuning was not an option as it requires significant resources, so we solved to use Parameter efficient fine tuning (PEFT). In PEFT, we further evaluated two approaches namely LoRA and QLoRA. In both of these approaches we take pretrained weights and freeze them. Then we inject trainable rank decomposition matrices in each layer of the transformer. QLoRA does another optimization on top of LoRa which further re- duces the memory footprint. It does a recoverable quantization of model parameters in 4 bits. We used two 3090 GPUs in the work.
