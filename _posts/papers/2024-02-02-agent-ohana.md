---
layout: paper
categories: papers
permalink: papers/agent-ohana
id: agent-ohana
title: "AgentOhana: Design Unified Data and Training Pipeline for Effective Agent Learning"
authors: 
  - Jianguo Zhang
  - Tian Lan
  - Ritheesh Murthy
  - Zhiwei Liu
  - Weiran Yao
  - Juntao Tan
  - Thai Hoang
  - Lianwei Yang
  - Yihao Feng
  - Zuxin Liu
  - Tulika Awalgaonkar
  - Juan Carlos Niebles
  - Silvio Savarese
  - Shelby Heinecke
  - Huan Wang
  - Caiming Xiong
venue: arXiv:2402.15506
venue-shorthand: arXiv
year: 2024
url: /papers/agent-ohana
pdf: https://arxiv.org/pdf/2402.15506
code: https://huggingface.co/Salesforce/xLAM-v0.1-r
featured: false
feature-title: AgentOhana
feature-description: Unified Data and Training Pipeline for Effective Agent Learning
selected: false
type: conference
figure: /images/papers/24-agent-ohana-arxiv.png
bibtex: |-

  @article{zhang2024agentohana,
      title={AgentOhana: Design Unified Data and Training Pipeline for Effective Agent Learning},
      author={Zhang, Jianguo and Lan, Tian and Murthy, Rithesh and Liu, Zhiwei and Yao, Weiran and Tan, Juntao and Hoang, Thai and Yang, Liangwei and Feng, Yihao and Liu, Zuxin and others},
      journal={arXiv preprint arXiv:2402.15506},
      year={2024}
  }
---

Autonomous agents powered by large language models (LLMs) have garnered significant research attention. However, fully harnessing the potential of LLMs for agent-based tasks presents inherent challenges due to the heterogeneous nature of diverse data sources featuring multi-turn trajectories. In this paper, we introduce **AgentOhana** as a comprehensive solution to address these challenges. *AgentOhana* aggregates agent trajectories from distinct environments, spanning a wide array of scenarios. It meticulously standardizes and unifies these trajectories into a consistent format, streamlining the creation of a generic data loader optimized for agent training. Leveraging the data unification, our training pipeline maintains equilibrium across different data sources and preserves independent randomness across devices during dataset partitioning and model training. Additionally, we present **xLAM-v0.1**, a large action model tailored for AI agents, which demonstrates exceptional performance across various benchmarks. Begin the exploration at [this URL](https://huggingface.co/Salesforce/xLAM-v0.1-r).
