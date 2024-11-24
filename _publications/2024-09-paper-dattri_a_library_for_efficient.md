---
title: "_dattri_: A Library for Efficient Data Attribution"
authors: "Junwei Deng\*, Ting Wei Li\*, Shiyuan Zhang, **Shixuan Liu**, Yijun Pan, Hao Huang, Xinhe Wang, Pingbang Hu, Xingjian Zhang, Jiaqi Ma"
collection: publications
category: conferences
permalink: /publication/2024-09-paper-dattri_a_library_for_efficient
excerpt: '**data attribution**, **data-centric AI**, **benchmark**'
date: 2024-11-13
venue: 'Neurips'
paperurl: 'http://sx-liu.github.io/files/2024-09-paper-dattri_a_library_for_efficient.pdf'
citation: # 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

**Abstract:** Data attribution methods aim to quantify the influence of individual training samples on the prediction of artificial intelligence (AI) models. As training data plays an increasingly crucial role in the modern development of large-scale AI models, data attribution has found broad applications in improving AI performance and safety. However, despite a surge of new data attribution methods being developed recently, there lacks a comprehensive library that facilitates the development, benchmarking, and deployment of different data attribution methods. In this work, we introduce dattri, an open-source data attribution library that addresses the above needs. Specifically, dattri highlights three novel design features. Firstly, dattri proposes a unified and easy-to-use API, allowing users to integrate different data attribution methods into their PyTorch-based machine learning pipeline with a few lines of code changed. Secondly, dattri modularizes low-level utility functions that are commonly used in data attribution methods, such as Hessian vector product, inverse-Hessian-vector product or random projection, making it easier for researchers to develop new data attribution methods. Thirdly, dattri provides a comprehensive benchmark framework with pre-trained models and ground truth annotations for a variety of benchmark settings, including generative AI settings. We have implemented a variety of state-of-the-art efficient data attribution methods that can be applied to large-scale neural network models, and will continuously update the library in the future. Using the developed dattri library, we are able to perform a comprehensive and fair benchmark analysis across a wide range of data attribution methods. The source code of dattri is available at [https://github.com/TRAIS-Lab/dattri](https://github.com/TRAIS-Lab/dattri).