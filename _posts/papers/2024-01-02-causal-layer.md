---
layout: paper
categories: papers
permalink: papers/causal-layer
id: causal-layer
title: "Causal Layering via Conditional Entropy"
authors: 
  - Itai Feigenbaum
  - Devansh Arpit
  - Shelby Heinecke
  - Juan Carlos Niebles
  - Weiran Yao
  - Caiming Xiong
  - Silvio Savarese
  - Huan Wang
venue: Proceedings of the Third Conference on Causal Learning and Reasoning
venue-shorthand: CLeaR
year: 2024
url: /papers/agent-ohana
pdf: https://proceedings.mlr.press/v236/feigenbaum24a/feigenbaum24a.pdf
featured: false
feature-title: Causal Layering
feature-description: Causal Layering via Conditional Entropy
selected: false
type: conference
figure: /images/papers/24-causal-layer-clear.png
bibtex: |-
  
  @inproceedings{feigenbaum2024causal,
    title={Causal Layering via Conditional Entropy},
    author={Feigenbaum, Itai and Arpit, Devansh and Heinecke, Shelby and Niebles, Juan Carlos and Yao, Weiran and Xiong, Caiming and Savarese, Silvio and Wang, Huan},
    booktitle={Proceedings of the Third Conference on Causal Learning and Reasoning},
    year={2024}
  }
---

Causal discovery aims to recover information about an unobserved causal graph from the observable data it generates. Layerings are orderings of the variables which place causes before effects. In this paper, we provide ways to recover layerings of a graph by accessing the data via a conditional entropy oracle, when distributions are discrete. Our algorithms work by repeatedly removing sources or sinks from the graph. Under appropriate assumptions and conditioning, we can separate the sources or sinks from the remainder of the nodes by comparing their conditional entropy to the unconditional entropy of their noise. Our algorithms are provably correct and run in worst-case quadratic time. The main assumptions are faithfulness and injective noise, and either known noise entropies or weakly monotonically increasing noise entropies along directed paths. In addition, we require one of either a very mild extension of faithfulness, or strictly monotonically increasing noise entropies, or expanding noise injectivity to include an additional single argument in the structural functions.
