---
layout: paper
categories: papers
permalink: papers/agentlite
id: xlam
title: "AgentLite: A Lightweight Library for Building and Advancing Task-Oriented LLM Agent System"
authors:
  - Zhiwei Liu
  - Weiran Yao
  - Jianguo Zhang
  - Liangwei Yang
  - Zuxin Liu
  - Juntao Tan
  - Prafulla Kumar Choubey
  - Tian Lan
  - Jason Wu
  - Huan Wang
  - Shelby Heinecke
  - Caiming Xiong
  - Silvio Savarese
equal-contribution:
  - Zhiwei Liu
  - Weiran Yao
venue: arXiv:2402.15538
venue-shorthand: arXiv
year: 2024
url: /papers/agentlite
pdf: https://arxiv.org/pdf/2402.15538
award: Dreamforce 2024
highlight: Databrick + AI Summit
code: https://github.com/SalesforceAIResearch/AgentLite
talk: https://www.salesforce.com/plus/experience/dreamforce_2024/series/the_future_of_ai_at_dreamforce_2024/episode/episode-s1e21?t=1310
demo: https://www.salesforce.com/plus/experience/dreamforce_2024/series/the_future_of_ai_at_dreamforce_2024/episode/episode-s1e21?t=1667 
preview: https://raw.githubusercontent.com/SalesforceAIResearch/AgentLite/main/image/weather_agent.gif
feature-title: Multiple Agents
feature-description: Salesforce's In-House Library for Multi-Agent Orchestration and Reasoning
image: /images/featured/agentlite.png
feature-order: 3
featured: true
selected: true
type: conference
figure: /images/papers/24-agentlite-arxiv.jpg
bibtex: |-

  @article{liu2024agentlite,
    title={AgentLite: A Lightweight Library for Building and Advancing Task-Oriented LLM Agent System},
    author={Liu, Zhiwei and Yao, Weiran and Zhang, Jianguo and Yang, Liangwei and Liu, Zuxin and Tan, Juntao and Choubey, Prafulla K and Lan, Tian and Wu, Jason and Wang, Huan and others},
    journal={arXiv preprint arXiv:2402.15538},
    year={2024}
  }

---

The booming success of LLMs initiates rapid development in LLM agents. Though the foundation of an LLM agent is the generative model, it is critical to devise the optimal reasoning strategies and agent architectures. Accordingly, LLM agent research advances from the simple chain-of-thought prompting to more complex ReAct and Reflection reasoning strategy; agent architecture also evolves from single agent generation to multi-agent conversation, as well as multi-LLM multi-agent group chat. However, with the existing intricate frameworks and libraries, creating and evaluating new reasoning strategies and agent architectures has become a complex challenge, which hinders research investigation into LLM agents. Thus, we open-source a new AI agent library, AgentLite, which simplifies this process by offering a lightweight, user-friendly platform for innovating LLM agent reasoning, architectures, and applications with ease. AgentLite is a task-oriented framework designed to enhance the ability of agents to break down tasks and facilitate the development of multi-agent systems. Furthermore, we introduce multiple practical applications developed with AgentLite to demonstrate its convenience and flexibility. Get started now at: [this URL](https://github.com/SalesforceAIResearch/AgentLite).

