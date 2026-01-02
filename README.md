# GLoMar: Benchmarking Web Retrieval in LLMs in Global and Local Marathi Contexts
## Abstract

The integration of web search and retrieval mechanisms into Large Language Models (LLMs) has significantly expanded their applicability in information-intensive and time-sensitive settings, yet their effectiveness in low-resource languages remains poorly understood. We study this gap through \textit{GLoMar}, a benchmark designed to evaluate internal LLM web retrieval for dynamic information access in Marathi. GLoMar distinguishes translated global queries from genuinely local, region-specific information needs, enabling fine-grained analysis of retrieval behaviour, accuracy, depth, and cost. We evaluate two frontier LLMs, GPT and Claude, against an external Google-based retrieval baseline and conduct detailed analyses of retrieval depth, error types, and cost–accuracy trade-offs. Our results show that while models reliably invoke web retrieval for Marathi queries, accuracy degrades sharply, particularly for local content, with most failures occurring during evidence interpretation. Shallow retrieval emerges as both the most accurate and cost-efficient strategy. GLoMar highlights critical limitations of current LLM-native retrieval in low-resource settings and provides a practical benchmark for future retrieval-centric research.

<div align="center">
  <img width="500" alt="Web_Img1" src="https://github.com/user-attachments/assets/f4c5841d-b8aa-45f5-b3fa-e2bcb7c1e095" />
</div>
</br>
*End-to-end evaluation pipeline covering uncertainty assessment, query issuance, retrieval outcomes, and accuracy transitions.*

## Overview

This repository accompanies our paper evaluating how closed-source LLMs decide when to invoke built-in web search, whether retrieval yields correct answers, and how cost scales with accuracy improvements.

## Method:

- Global split: evaluates selective invocation based on globall translated Marathi queries.
- Local split: evaluates whether models detect information staleness and fetch updated answers for local Marathi queries.
- Metrics: accuracy, calibration impact, cost per improvement, and query efficiency.
- Models tested: Claude 4.5 Haiku and GPT-5-mini.


## Citation

A BibTeX entry will be added after acceptance!
