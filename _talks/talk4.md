---
title: "Accurate and Predictable Scoring for Hardware Contention in Microservices"
collection: talks
type: "Talk"
venue: "Industry Research Talk"
date: 2025-12-18
location: "Tufts University"
---

This talk presents a practical approach to quantifying and forecasting hardware contention in microservices so mitigation can happen before SLO violations. It motivates why contention remains underappreciated in containerized systems, introduces a general contention score (0-1) designed around four properties (correlation with latency degradation, sharp rise, slow decay, and predictability), and describes the Gordion pipeline: workload/stress generation (`wrk2` + `stress-ng`), multi-layer instrumentation (within-service gRPC timing plus `perf` counters), score labeling, and ML-based next-step prediction. The evaluation highlights both usefulness and deployability, including competitive prediction quality and low runtime overhead near saturation (about 1% mean and 8% P90 at 500 RPS). Slides: [(Industry) Accurate and Predictable Scoring for Hardware Contention in Microservices](https://docs.google.com/presentation/d/1AoVLX1oqhDnEIJrs5cYbQNyB8p6iEmdFAPhK2KUTwj8/edit?usp=sharing).