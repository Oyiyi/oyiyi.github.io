---
title: "FinCriticalED: A Visual Benchmark for Financial Fact-Level OCR Evaluation"
collection: publications
category: manuscripts
permalink: /publication/2025-10-files-fincriticaled-a-visual-benchmark-for-financial-fact-level-ocr-evaluation
excerpt: 'FinCriticalED (Financial Critical Error Detection), a visual benchmark for evaluating OCR (Optical Character Recognition) and vision language models on financial documents at the fact level, providing 500 image-HTML pairs with expert annotated financial facts covering over seven hundred numerical and temporal facts.'
date: 2025-09-19
venue: 'CVPR 2026 Conference Submission'
# slidesurl: 'http://oyiyi.github.io/files/slides1.pdf'
# paperurl: 'http://oyiyi.github.io/files/FinCriticalED.pdf'
arxivurl: 'https://arxiv.org/abs/2511.14998'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
We introduce FinCriticalED (Financial Critical Error Detection), a visual benchmark for evaluating OCR and vision language models on financial documents at the fact level. Financial documents contain visually dense and table heavy layouts where numerical and temporal information is tightly coupled with structure. In high stakes settings, small OCR mistakes such as sign inversion or shifted dates can lead to materially different interpretations, while traditional OCR metrics like ROUGE and edit distance capture only surface level text similarity.

FinCriticalED provides 500 image-HTML pairs with expert annotated financial facts covering over seven hundred numerical and temporal facts. It introduces three key contributions. First, it establishes the first fact level evaluation benchmark for financial document understanding, shifting evaluation from lexical overlap to domain critical factual correctness. Second, all annotations are created and verified by financial experts with strict quality control over signs, magnitudes, and temporal expressions. Third, we develop an LLM-as-Judge evaluation pipeline that performs structured fact extraction and contextual verification for visually complex financial documents.

We benchmark OCR systems, open source vision language models, and proprietary models on FinCriticalED. Results show that although the strongest proprietary models achieve the highest factual accuracy, substantial errors remain in visually intricate numerical and temporal contexts. Through quantitative evaluation and expert case studies, FinCriticalED provides a rigorous foundation for advancing visual factual precision in financial and other precision critical domains.
