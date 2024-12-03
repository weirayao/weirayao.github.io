---
layout: paper
categories: papers
permalink: papers/distribution
id: distribution
title: "Distribution-aware Goal Prediction and Conformant Model-based Planning for Safe Autonomous Driving
"
authors:
  - Jonathan Francis
  - Bingqing Chen
  - Weiran Yao
  - Eric Nyberg
  - Jean Og
venue: International Conference on Machine Learning
venue-shorthand: ICML
location: Baltimore, Maryland USA
year: 2022
url: /papers/distribution
pdf: https://arxiv.org/pdf/2212.08729
talk: https://icml.cc/virtual/2022/20892
slides: https://slideslive.com/38987757/distributionaware-goal-prediction-and-conformant-modelbased-planning-for-safe-autonomous-driving
blog: https://icml.cc/virtual/2022/workshop/13475
featured: false
feature-title: Learning to Drive
feature-description: Distribution-aware Goal Prediction and Conformant Model-based Planning for Safe Autonomous Driving
selected: true
type: conference
award: Best Paper Award
bibtex: |-

    @article{francis2022distribution,
        title={Distribution-aware Goal Prediction and Conformant Model-based Planning for Safe Autonomous Driving},
        author={Francis, Jonathan and Chen, Bingqing and Yao, Weiran and Nyberg, Eric and Oh, Jean},
        journal={arXiv preprint arXiv:2212.08729},
        year={2022}
    }

---

The feasibility of collecting a large amount of expert demonstrations has inspired growing research interests in learning-to-drive settings, where models learn by imitating the driving behaviour from experts. However, exclusively relying on imitation can limit agents' generalisability to novel scenarios that are outside the support of the training data. In this paper, we address this challenge by factorising the driving task, based on the intuition that modular architectures are more generalisable and more robust to changes in the environment compared to monolithic, end-to-end frameworks. Specifically, we draw inspiration from the trajectory forecasting community and reformulate the learning-to-drive task as obstacle-aware perception and grounding, distribution-aware goal prediction, and model-based planning. Firstly, we train the obstacle-aware perception module to extract salient representation of the visual context. Then, we learn a multi-modal goal distribution by performing conditional density-estimation using normalising flow. Finally, we ground candidate trajectory predictions road geometry, and plan the actions based on on vehicle dynamics. Under the CARLA simulator, we report state-of-the-art results on the CARNOVEL benchmark.
