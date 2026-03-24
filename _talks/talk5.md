---
title: "Automatically Identifying Errant Upstream Contention Triggers in Microservice-based Applications"
collection: talks
type: "Talk"
venue: "Industry Research Talk"
date: 2024-12-20
location: "Tufts University"
---

This talk presents `OrthoView`, a tracing-based method for diagnosing errant upstream contention triggers in microservice applications, where user-visible slowdowns are caused or sustained by problematic upstream request behaviors rather than only local service issues. The presentation frames the problem through victim/survivor differentiation under SLO violations, then walks through a stepwise pipeline: heavy-hitter edge detection on critical paths, temporal-overlap aggressor discovery, and backtrace feature scoring/ranking to identify likely problematic contention triggers and assess whether they are truly errant. It also covers implementation and evaluation on a large TrainTicket testbed under controlled bursty-load scenarios, highlighting initial effectiveness and practical next steps around tracing-overhead control and sampling strategies. 

Slides: [CACTI-CGM-postICPE](https://docs.google.com/presentation/d/1ukfoXwgyEsC7ZNHOSoZKkUWJNIpv-QjbcwIMHHcGt9A/edit?usp=sharing).