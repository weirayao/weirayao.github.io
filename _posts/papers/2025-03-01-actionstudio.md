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

Personalization is critical in AI assistants, particularly in the context of private AI models that work with individual users. A key scenario in this domain involves enabling AI models to access and interpret a user's private data (e.g., conversation history, user-AI interactions, app usage) to understand personal details such as biographical information, preferences, and social connections. However, due to the sensitive nature of such data, there are no publicly available datasets that allow us to assess an AI model's ability to understand users through direct access to personal information.
To address this gap, we introduce a synthetic data generation pipeline that creates diverse, realistic user profiles and private documents simulating human activities. Leveraging this synthetic data, we present PersonaBench, a benchmark designed to evaluate AI models' performance in understanding personal information derived from simulated private user data.

We evaluate Retrieval-Augmented Generation (RAG) pipelines using questions directly related to a user's personal information, supported by the relevant private documents provided to the models. Our results reveal that current retrieval-augmented AI models struggle to answer private questions by extracting personal information from user documents, highlighting the need for improved methodologies to enhance personalization capabilities in AI.
