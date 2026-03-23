---
title: "Automating instrumentation choices for performance problems in distributed applications with VAIF"
collection: publications
permalink: /publications/vaif
excerpt: "VAIF automatically selects low-overhead distributed tracing instrumentation to localize performance problems in systems like OpenStack and HDFS."
date: 2021-10-01
venue: 'ACM SOSP 2021'
classes: wide
---

## Abstract
Developers use logs to diagnose performance problems in distributed applications. However, it is difficult to know a priori where logs are needed and what information in them is needed to help diagnose problems that may occur in the future. We present the Variance-driven Automated Instrumentation Framework (VAIF), which runs alongside distributed applications. In response to newly-observed performance problems, VAIF automatically searches the space of possible instrumentation choices to enable the logs needed to help diagnose them. To work, VAIF combines distributed tracing (an enhanced form of logging) with insights about how response-time variance can be decomposed on the critical-path portions of requests' traces. We evaluate VAIF by using it to localize performance problems in OpenStack and HDFS. We show that VAIF can localize problems related to slow code paths, resource contention, and problematic third-party code while enabling only 3-34% of the total tracing instrumentation.

[Download paper here](https://dl.acm.org/doi/10.1145/3472883.3487000)
