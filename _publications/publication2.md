---
title: "(Poster) Diagnosing behavioral causes of contention in distributed systems"
collection: publications
permalink: /publications/cacti_poster
excerpt: "We outline a tracing-based method to diagnose contention in distributed systems by localizing victim requests, finding temporally overlapping concurrent traces as candidate aggressors, and iteratively enabling contention-focused tracepoints."
date: 2023-04-15
venue: 'USENIX NSDI'
authorship: "1st author"
classes: wide
---

### Summary

Debugging contention in distributed applications is hard: engineers must either log very broadly (expensive and especially costly under contention) or instrument narrowly without knowing in advance which layers and behaviors matter, while cross-layer resource effects are often opaque. Prior tracing systems either impose impractical overhead when aggressively sampling contention (e.g., Zeno) or focus on a single poorly performing request type and miss cross-request interactions (e.g., Hindsight, VAIF).

Our work starts from two ideas: contention diagnosis needs **tail-based** tracing so we can search for “victim” requests (slow or high-variance regions in traces), and **wall-clock overlap** among queue-style contention lets us relate concurrent traces to those victims. Building on **VAIF**’s automated tracepoint enabling/disabling, we describe a four-step workflow: (1) localize a victim trace segment affected by contention; (2) discover **candidate aggressors**—concurrent trace segments that overlap the victim in time; (3) explain contention by analyzing commonality in call hierarchy between candidates and the victim to identify true contributors; and (4) **iteratively enable** additional tracepoints on aggressors to refine diagnosis without turning on full-application instrumentation.

We also discuss supporting mechanisms we are designing: a storage and indexing scheme for trace segments to query temporal overlaps efficiently at runtime, grouping and filtering candidates (e.g., by request type, host, or fine-grained key–value properties) to reduce spurious correlations, and using aggressive filtering before maximal localization to keep overhead manageable on already contended systems.

