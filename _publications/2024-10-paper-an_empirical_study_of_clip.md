---
title: "An empirical study of CLIP fine-tuning with similarity clusters"
collection: publications
category: workshops
permalink: /publication/2024-10-paper-an_empirical_study_of_clip
excerpt: '**multimodal representation learning**, **visual representation learning**, **CLIP fine-tuning**'
date: 2024-02-17
venue: 'FITML @ Neurips 2024'
paperurl: 'http://sx-liu.github.io/files/2024-10-paper-an_empirical_study_of_clip.pdf'
citation: # 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

**Abstract:** With the success of CLIP training for learning transferable visual representations, fine-tuning CLIP models on smaller datasets for better downstream performance is an important area of research. A method for improving CLIP models is to increase the difficulty of negative examples. While the majority of research has focused on manually crafting hard negative captions, this strategy requires additional engineering labor, fails to generalize to different domains, and causes additional overfitting. Here, we conduct an empirical study to systematically explore an alternative approach: construct minibatches that include similarity clusters to increase the difficulty of negative examples. We propose a generalized framework, called SimCLIP, for similarity-based CLIP fine-tuning. By enforcing that each minibatch contains clusters of similar examples, SimCLIP fine-tuning can improve model performance compared to standard CLIP fine-tuning. We extensively study which SimCLIP configurations and factors contribute most to downstream performance. We also analyze SimCLIP’s performance on rare special sets, compositionality of attributes, and generalization across dataset sizes. Our observations provides better understanding of similarity-based minibatch construction methods as well as new insights into CLIP fine-tuning. The code for our experiments is available at https://github.com/sx-liu/SimCLIP/
