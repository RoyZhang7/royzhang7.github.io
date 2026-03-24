---
title: "(Guest Lecture) TA's Journey of Solving OS Research Questions"
collection: talks
type: "Guest Lecture"
venue: "Operating System Course"
date: 2024-11-04
location: "Tufts University"
---

This guest lecture walks through a systems-research journey from distributed tracing in user space to debugging invisible kernel- and hardware-level bottlenecks in microservices, highlighting why request context is lost at kernel boundaries and how that limits cross-layer diagnosis. The talk compares three context-propagation approaches—extra syscalls, eBPF-based propagation/maps/ring buffers, and customized syscall hooks inspired by Zpoline—and discusses their trade-offs in overhead, maintainability, and observability, with the practical takeaway that efficient context propagation plus low-overhead kernel-to-user data paths are key to scalable vertical tracing.
Slides: [TA's journey of solving OS research questions](https://docs.google.com/presentation/d/1UOvodte9ZM6RjPISiLPUfUcboJmX1o1Fe9TpJkVthBM/edit?usp=sharing).