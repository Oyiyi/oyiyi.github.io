---
title: "Finetune Foundational Model"
excerpt: "Exploring the Limits of Fine-Tuning in Language Adaptation for Large<br/><br/>
The emergence of Large Language Models over the past few years has enabled new applications of natural language tasks, specifically in the field of language adaptation. It is computationally expensive to train new Large Language Models from scratch due to the billions of parameters in these state of the art models and the scale of training data. <br/><br/>

From our inference trials, the newly launched Meta-Llama-3-8B-Instruct (April, 2024) doesn’t do well in conversations in languages other than English. In this work, we present a method to fine-tune different base models trained primarily on English text to adapt the model for Q&A for the Chinese and Turkish language.<br/><br/>

The objective was to create custom foreign language agents from the base model using fine-tuning. Full fine-tuning was not an option as it requires significant resources, so we solved to use Parameter efficient fine tuning (PEFT). In PEFT, we further evaluated two approaches namely LoRA and QLoRA. In both of these approaches we take pretrained weights and freeze them. Then we inject trainable rank decomposition matrices in each layer of the transformer. QLoRA does another optimization on top of LoRa which further re- duces the memory footprint. It does a recoverable quantization of model parameters in 4 bits. We used two 3090 GPUs in the work.<br/><br/>
"
collection: portfolios-competitions
---

This is an item in your portfolio. It can be have images or nice text. If you name the file .md, it will be parsed as markdown. If you name the file .html, it will be parsed as HTML. 
