---
title: "_dattri-LLM_: A Unified and Efficient Library for Training Data Attribution at LLM Scale"
authors: "**Shixuan Liu**, Tongli Zhou, Junwei Deng, Pingbang Hu, Jiaqi W. Ma"
collection: publications
category: preprints
permalink: /publication/2026-09-paper-dattri_llm_a_unified_and_efficient
excerpt: '**data attribution**, **large language models**, **open-source library**'
date: 2026-09-30
venue: 'arXiv'
paperurl: 'https://arxiv.org/abs/2609.38767'
citation: # 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

**Abstract:** Training data attribution (TDA) estimates the contribution of individual training examples to model outputs. Most scalable TDA methods rely on per-example gradients, whose computation and use at LLM scale pose challenges in efficiency, compatibility, and extensibility. We introduce dattri-LLM, a TDA library that makes gradient-based attribution more practical at scale. For efficiency, dattri-LLM uses compact gradient representations and dynamically routes gradient operations based on a cost model. For compatibility, its capture mechanism collects per-example gradients from existing training loops that call backward(), without requiring changes to the loop or its configuration. This includes distributed training with DDP and FSDP and pipelines built with HuggingFace Transformers, TRL, and OLMo. For extensibility, dattri-LLM exposes reusable gradient operations and training-time callbacks for implementing attribution methods and applications. These interfaces support a variety of attribution methods, including gradient similarity, curvature-based influence, and trajectory-based methods, as well as applications that act on gradients during training, such as online data selection. On the same hardware and workload, dattri-LLM achieves 3.2x the throughput of the fastest competing library on average, scales multiple attribution methods to 110B-parameter models across four H200 GPUs, and offers superior attribution fidelity-cost trade-offs across a range of models with different model families and scales. The source code of dattri-LLM is available at [https://github.com/TRAIS-Lab/dattri-llm](https://github.com/TRAIS-Lab/dattri-llm).
