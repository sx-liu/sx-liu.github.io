---
title: "RL-IF: Tracking Non-local Training Data Influence for Online Reinforcement Learning"
authors: "**Shixuan Liu**\\*, Cheng Tang\\*, Yuzheng Hu\\*, Fan Wu, Han Zhao, Jiaqi W. Ma"
collection: publications
category: conferences
permalink: /publication/2026-10-paper-rl_if_tracking_non_local
excerpt: '**data attribution**, **reinforcement learning**, **data selection**'
date: 2026-10-20
venue: 'NeurIPS'
paperurl: 'https://arxiv.org/abs/2610.28883'
citation: # 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

**Abstract:** Online reinforcement learning (RL) has achieved significant success in decision-making tasks, but modern online RL remains highly sensitive to the quality of training experience. Understanding the contribution of individual training instances is therefore central to data-centric RL, with applications ranging from experience selection to policy interpretation. Existing data attribution methods for online RL primarily focus on local influence within a single training round, overlooking the non-local data influence across multiple training rounds. In this work, we formalize data attribution in online RL through a trajectory-level leave-one-out quantity, RL-LOO, which measures how one training sample influences a downstream target after subsequent online updates have taken place. We then derive RL-IF, a first-order estimator that propagates data influence through both optimization effects and policy-induced sampling effects, and provide theoretical guarantees on its approximation accuracy under smoothness assumptions. Our analysis further disentangles these two effects and shows both theoretically and empirically that the full RL-IF estimator can often be well approximated using the optimization effect alone. Building on this observation, we develop RINSE, a practical data filtering method for online RL. Experiments on standard control benchmarks and an RLHF-style toxicity-mitigation setting show that RINSE improves training efficiency and final performance over standard PPO and local attribution baselines. These results suggest that RL-IF provides a practical and principled framework for understanding and improving online RL.
