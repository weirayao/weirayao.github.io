---
layout: paper
categories: papers
permalink: papers/actionstudio
id: actionstudio
title: "ActionStudio: A Lightweight Framework for Data and Training of Large Action Models"
authors:
  - Jianguo Zhang
  - Thai Hoang
  - Ming Zhu
  - Zuxin Liu
  - Shiyu Wang
  - Tulika Awalgaonkar
  - Akshara Prabhakar
  - Haolin Chen
  - Weiran Yao
  - Zhiwei Liu
  - Juntao Tan
  - Juan Carlos Niebles
  - Shelby Heinecke
  - Huan Wang
  - Silvio Savarese
  - Caiming Xiong

venue: arXiv
venue-shorthand: arXiv
year: 2025
pdf: https://arxiv.org/pdf/2503.22673
feature-title: ActionStudio
feature-description: A Highly-Parallelized Training Framework for AI Agents
featured: false
selected: false
type: conference
bibtex: |-

    @article{zhang2025actionstudio,
      title={ActionStudio: A Lightweight Framework for Data and Training of Large Action Models},
      author={Zhang, Jianguo and Hoang, Thai and Zhu, Ming and Liu, Zuxin and Wang, Shiyu and Awalgaonkar, Tulika and Prabhakar, Akshara and Chen, Haolin and Yao, Weiran and Liu, Zhiwei and others},
      journal={arXiv e-prints},
      pages={arXiv--2503},
      year={2025}
    }

---

Action models are essential for enabling autonomous agents to perform complex tasks. However, training large action models remains challenging due to the diversity of agent environments and the complexity of agentic data. Despite growing interest, existing infrastructure provides limited support for scalable, agent-specific fine-tuning. We present ActionStudio, a lightweight and extensible data and training framework designed for large action models. ActionStudio unifies heterogeneous agent trajectories through a standardized format, supports diverse training paradigms including LoRA, full fine-tuning, and distributed setups, and integrates robust preprocessing and verification tools. We validate its effectiveness across both public and realistic industry benchmarks, demonstrating strong performance and practical scalability. We open-sourced code and data at this https URL to facilitate research in the community.
