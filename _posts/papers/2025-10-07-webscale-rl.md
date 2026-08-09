---
layout: paper
categories: papers
permalink: papers/webscale-rl
id: webscale-rl
title: "Webscale-RL: Automated Data Pipeline for Scaling RL Data to Pretraining Levels"
authors:
  - Zhepeng Cen
  - Haolin Chen
  - Shiyu Wang
  - Zuxin Liu
  - Zhiwei Liu
  - Jielin Qiu
  - Ding Zhao
  - Silvio Savarese
  - Caiming Xiong
  - Huan Wang
  - Weiran Yao
corresponding-author:
  - Huan Wang
  - Weiran Yao
venue: arXiv
venue-shorthand: arXiv
year: 2025
url: /papers/webscale-rl
pdf: https://arxiv.org/pdf/2510.06499
code: https://huggingface.co/datasets/Salesforce/Webscale-RL
featured: false
selected: true
type: conference
bibtex: |-

    @article{cen2025webscale,
      title={Webscale-RL: Automated Data Pipeline for Scaling RL Data to Pretraining Levels},
      author={Cen, Zhepeng and Chen, Haolin and Wang, Shiyu and Liu, Zuxin and Liu, Zhiwei and Qiu, Jielin and Zhao, Ding and Savarese, Silvio and Xiong, Caiming and Wang, Huan and Yao, Weiran},
      journal={arXiv preprint arXiv:2510.06499},
      year={2025}
    }
---

Large Language Models (LLMs) have achieved remarkable success through imitation learning on vast text corpora, but this paradigm creates a training-generation gap and limits robust reasoning. Reinforcement learning (RL) offers a more data-efficient solution capable of bridging this gap, yet its application has been constrained by a critical data bottleneck: existing RL datasets are orders of magnitude smaller and less diverse than web-scale pre-training corpora. To address this, we introduce the Webscale-RL pipeline, a scalable data engine that systematically converts large-scale pre-training documents into millions of diverse, verifiable question-answer pairs for RL. Using this pipeline, we construct the Webscale-RL dataset, containing 1.2 million examples across more than 9 domains. Our experiments show that the model trained on this dataset significantly outperforms continual pretraining and strong data refinement baselines across a suite of benchmarks. Notably, RL training with our dataset proves substantially more efficient, achieving the performance of continual pre-training with up to 100× fewer tokens. Our work presents a viable path toward scaling RL to pre-training levels, enabling more capable and efficient language models.
