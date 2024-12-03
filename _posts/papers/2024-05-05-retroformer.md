---
layout: paper
categories: papers
permalink: papers/retroformer
id: retroformer
title: "Retroformer: Retrospective Large Language Agents with Policy Gradient Optimization"
authors: 
  - Weiran Yao
  - Shelby Heinecke
  - Juan Carlos Niebles
  - Zhiwei Liu
  - Yihao Feng
  - Le Xue
  - Rithesh Murthy
  - Zeyuan Chen
  - Jianguo Zhang
  - Devansh Arpit
  - Ran Xu
  - Phil Mui
  - Huan Wang
  - Caiming Xiong
  - Silvio Savarese
venue: International Conference on Learning Representations
venue-shorthand: ICLR
location: Vienna, Austria
year: 2024
url: /papers/retroformer
award: Spotlight Presentation, Top 5% Paper
pdf: https://arxiv.org/pdf/2308.02151
talk: https://iclr.cc/virtual/2024/poster/18908
code: https://github.com/weirayao/Retroformer
slides: https://docs.google.com/presentation/d/1TMbv5zaFUW9RV45vzJPtvgbwhXEg82q1rviWS7t3CQM/edit?usp=sharing
featured: true
image: /images/featured/retroformer.png
feature-title: Retroformer
feature-description: Generative Critic Model Optimized for Self-Reflection and Reasoning Capabilities of AI Agents
feature-order: 1
selected: true
type: conference
figure: /images/papers/24-retroformer-iclr.png
bibtex: |-

    @inproceedings{
      yao2024retroformer,
      title={Retroformer: Retrospective Large Language Agents with Policy Gradient Optimization},
      author={Weiran Yao and Shelby Heinecke and Juan Carlos Niebles and Zhiwei Liu and Yihao Feng and Le Xue and Rithesh R N and Zeyuan Chen and Jianguo Zhang and Devansh Arpit and Ran Xu and Phil L Mui and Huan Wang and Caiming Xiong and Silvio Savarese},
      booktitle={The Twelfth International Conference on Learning Representations},
      year={2024},
      url={https://openreview.net/forum?id=KOZu91CzbK}
    }
---

Recent months have seen the emergence of a powerful new trend in which large language models (LLMs) are augmented to become autonomous language agents capable of performing objective oriented multi-step tasks on their own, rather than merely responding to queries from human users. Most existing language agents, however, are not optimized using environment-specific rewards. Although some agents enable iterative refinement through verbal feedback, they do not reason and plan in ways that are compatible with gradient-based learning from rewards. This paper introduces a principled framework for reinforcing large language agents by learning a retrospective model, which automatically tunes the language agent prompts from environment feedback through policy gradient. Specifically, our proposed agent architecture learns from rewards across multiple environments and tasks, for fine-tuning a pre-trained language model which refines the language agent prompt by summarizing the root cause of prior failed attempts and proposing action plans. Experimental results on various tasks demonstrate that the language agents improve over time and that our approach considerably outperforms baselines that do not properly leverage gradients from the environment.
