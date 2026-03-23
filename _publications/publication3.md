---
title: "Accurate and Predictable Scoring for Hardware Contention in Microservices"
collection: publications
permalink: /publications/publication3
excerpt: "We introduce a mitigation-agnostic tanh-based contention score for microservices—implemented in the Gordion framework—and show it can be predicted from performance counters and within-service latencies so operators can act before SLO violations."
date: 2025-12-15
venue: 'In Prep'
authorship: "1st author"
publ: "false"
---

### Abstract

Microservices frequently suffer performance problems and outages due to contention for hardware resources. Prior work on mitigating contention often relies on heuristics, does not scale, or is tightly coupled to a single mitigation technique. We take a different approach and decouple mitigation from measurement; this paper is the first part of that agenda. We present a novel contention score that quantifies the contention level of a microservice and is general enough to drive any mitigation mechanism (e.g., autoscaling, rate limiting, diagnosis). The score is grounded in properties a usable score should satisfy so mitigations know when to act. We show that the score is easy to predict from performance counters and within-microservice latencies as features, enabling mechanisms to respond before severe outcomes. We trained five predictors with different ML models; RMSE ranged from 0.0827 to 0.1548, MAE from 0.0338 to 0.1162, and R² from 0.2240 to 0.7807.
