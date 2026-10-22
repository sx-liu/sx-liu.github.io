---
title: "Distilling Diffusion Score Discrepancy for Efficient Training Data Attribution"
authors: "**Shixuan Liu**, Joan Serrà, Kin Wai Cheuk, Jinju Kim, Woosung Choi, Yukara Ikemiya, Wei-Hsiang Liao, Jiaqi W. Ma, Yuki Mitsufuji"
collection: publications
category: preprints
permalink: /publication/2026-09-paper-distilling_diffusion_score_discrepancy
excerpt: '**data attribution**, **diffusion models**, **distillation**'
date: 2026-09-30
venue: 'arXiv'
paperurl: 'https://arxiv.org/abs/2609.38776'
citation: # 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

**Abstract:** Training data attribution for diffusion models aims to identify the training samples that influence a generated instance, but existing methods either require costly per-sample gradient computation or query-specific model optimization. Moreover, most methods attribute changes in a proxy loss rather than changes in the actual model's generative behavior. We address these limitations by formulating attribution directly with a local score discrepancy measure, which applies to any diffusion variant (including DDPM, EDM, and flow matching), and by showing that such measure can be estimated without retraining, as a preconditioned gradient similarity. We instantiate this estimator as Training-data Influence via score Discrepancy (TID), which uses Kronecker-factored curvature to avoid random projections and per-sample gradient storage. We then distill TID into TIDE, a forward-only student trained online to reproduce the teacher's rankings from the diffusion model's internal activations. Under counterfactual evaluation on CIFAR-10, ArtBench-10, and MS-COCO, TID matches or outperforms state-of-the-art approaches, while TIDE retains most of TID's accuracy at four to five orders of magnitude lower per-query cost, attributing generated samples in milliseconds and faster than the generation itself.
