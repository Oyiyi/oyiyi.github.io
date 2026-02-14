---
title: "FinTagging: An LLM-ready Benchmark for Extracting and Structuring Financial Information"
collection: publications
category: manuscripts
permalink: /publication/2025-05-files-fintagging-an-llm-ready-benchmark-for-extracting-and-structuring-financial-information
excerpt: 'FINTAGGING, the first full-scope, table-aware XBRL benchmark designed to evaluate the structured information extraction and semantic alignment capabilities of large language models (LLMs) in the context of XBRL-based financial reporting.'
date: 2025-05-27
venue: 'ACL ARR 2026 January Submission'
# slidesurl: 'http://oyiyi.github.io/files/slides1.pdf'
# paperurl: 'http://oyiyi.github.io/files/FinTagging-An LLM-ready Benchmark for Extracting and Structuring Financial Information.pdf'
arxivurl: 'https://arxiv.org/pdf/2505.20650'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
We introduce FINTAGGING, the first full-scope, table-aware XBRL benchmark designed to evaluate the structured information extraction and semantic alignment capabilities of large language models (LLMs) in the context of XBRL-based financial reporting. 

Unlike prior benchmarks that oversimplify XBRL tagging as flat multi-class classification and focus solely on narrative text, FINTAGGING decomposes the XBRL tagging problem into two subtasks: FinNI for financial entity extraction and FinCL for taxonomy-driven concept alignment. It requires models to jointly extract facts and align them with the full 10k+ US-GAAP taxonomy across both unstructured text and structured tables, enabling realistic, fine-grained evaluation. 

We assess a diverse set of LLMs under zero-shot settings, systematically analyzing their performance on both subtasks and overall tagging accuracy. Our results reveal that, while LLMs demonstrate strong generalization in information extraction, they struggle with fine-grained concept alignment, particularly in disambiguating closely related taxonomy entries. These findings highlight the limitations of existing LLMs in fully automating XBRL tagging and underscore the need for improved semantic reasoning and schema-aware modeling to meet the demands of accurate financial disclosure. Code is available at our GitHub repository1 and data is at our Hugging Face repository. 