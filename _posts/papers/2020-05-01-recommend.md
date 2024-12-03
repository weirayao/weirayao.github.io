---
layout: paper
categories: papers
permalink: papers/recommend
id: recommend
title: "Learning to Recommend Signal Plans under Incidents with Real-Time Traffic Prediction"
authors: 
  - Weiran Yao
  - Sean Qian
venue: "Transportation Research Record: Journal of the Transportation Research Board"
venue-shorthand: TRR
year: 2020
url: /papers/recommend
pdf: https://journals.sagepub.com/doi/abs/10.1177/0361198120917668
doi: https://doi.org/10.1177/0361198120917668
featured: false
selected: false
type: journal
feature-title: Signal
feature-description: Recommending Signal Plans under Incidents with Real-Time Traffic
bibtex: |-

    @article{yao2020learning,
        title={Learning to recommend signal plans under incidents with real-time traffic prediction},
        author={Yao, Weiran and Qian, Sean},
        journal={Transportation Research Record},
        volume={2674},
        number={6},
        pages={45--59},
        year={2020},
        publisher={SAGE Publications Sage CA: Los Angeles, CA}
    }
---

The main question to address in this paper is to recommend optimal signal timing plans in real time under incidents by incorporating domain knowledge developed with the traffic signal timing plans tuned for possible incidents, and learning from historical data of both traffic and implemented signals timing. The effectiveness of traffic incident management is often limited by the late response time and excessive workload of traffic operators. This paper proposes a novel decision-making framework that learns from both data and domain knowledge to real-time recommend contingency signal plans that accommodate non-recurrent traffic, with the outputs from real-time traffic prediction at least 30 min in advance. Specifically, considering the rare occurrences of engagement of contingency signal plans for incidents, it is proposed to decompose the end-to-end recommendation task into two hierarchical models—real-time traffic prediction and plan association. The connections between the two models are learnt through metric learning, which reinforces partial-order preferences observed from historical signal engagement records. The effectiveness of this approach is demonstrated by testing this framework on the traffic network in Cranberry Township, Pennsylvania, U.S., in 2019. Results show that the recommendation system has a precision score of 96.75% and recall of 87.5% on the testing plan, and makes recommendations an average of 22.5 min lead time ahead of Waze alerts. The results suggest that this framework is capable of giving traffic operators a significant time window to access the conditions and respond appropriately.