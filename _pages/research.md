---
title: "Research"
permalink: /research/
author_profile: true
---

My research focuses on **data-centric computer architecture and systems** for memory-intensive AI and high-performance computing (HPC) workloads. Across four complementary directions, I study how to characterize data-access and data-movement costs, exploit locality and concurrency, and match execution strategies with memory-system capabilities.

## Concurrency-Aware Memory-System Optimization

Modern memory hierarchies must handle diverse and evolving access patterns, yet conventional cache and prefetching policies often overlook the effects of concurrent data accesses on performance. This research develops concurrency-aware models and adaptive techniques for cache management, prefetching, and memory-hierarchy optimization. By combining memory-access concurrency, data locality, and runtime feedback, these methods aim to reduce exposed memory latency and improve performance across data-intensive workloads.

**Selected Publications**

- [ACES – Accelerating Sparse Matrix Multiplication with Adaptive Execution Flow and Concurrency-Aware Cache Optimizations (ASPLOS 2024)](../publications/ASPLOS2024)
- [CHROME – Concurrency-Aware Holistic Cache Management Framework with Online Reinforcement Learning (HPCA 2024)](../publications/HPCA2024)
- [CARE – A Concurrency-Aware Enhanced Lightweight Cache Management Framework (HPCA 2023)](../publications/HPCA2023)
- [APAC – An Accurate and Adaptive Prefetch Framework with Concurrent Memory Access Analysis (ICCD 2020)](../publications/ICCD2020)

---

## Performance and I/O Modeling

Understanding data-access and data-movement costs is essential for optimizing memory-intensive AI and HPC workloads. This research develops analytical models of hierarchical memory performance and I/O complexity to identify bottlenecks, establish fundamental performance limits, and guide algorithm and system design. The resulting models connect workload requirements with architecture-level decisions, from concurrency-aware memory performance to long-sequence attention and processing-in-memory (PIM) design-space exploration.

**Selected Publications**

- [PILOT – I/O-Aware PIM Acceleration for Long-Sequence LLM Inference with Hybrid Sparse Attention (IPDPS 2026)](../publications/IPDPS2026)
- [AttenIO – I/O Analysis is All You Need: An I/O Analysis for Long-Sequence Attention (ASPLOS 2026)](../publications/ASPLOS2026)
- [The Memory-Bounded Speedup Model and its Impacts in Computing (JCST 2023)](../publications/JCST2023)
- [A Generalized Model For Modern Hierarchical Memory System (WSC 2022)](../publications/WSC2022)

---

## Learning-Assisted System Optimization

As workloads and hardware resource constraints become increasingly diverse, static optimization policies cannot always sustain high performance. This research applies reinforcement learning and lightweight machine-learning methods to predict memory behavior and guide adaptive system and execution decisions. Applications include cache management, secure-memory counter caching, and reuse-aware GPU block scheduling, combining online adaptation and offline learning with an emphasis on performance efficiency and practical runtime overhead.

**Selected Publications**

- [Ziggs – Improving Data Reuse across Blocks for Efficient Block-Sparse Transformers on GPUs (PACT 2026)](../publications/PACT2026)
- [COSMOS – RL-Enhanced Locality-Aware Counter Cache Optimization for Secure Memory (MICRO 2025)](../publications/MICRO2025)
- [CAMP – Concurrency-Aware Cache Miss Cost Prediction with Perceptron Learning (GLSVLSI 2025)](../publications/GLSVLSI2025)
- [CHROME – Concurrency-Aware Holistic Cache Management Framework with Online Reinforcement Learning (HPCA 2024)](../publications/HPCA2024)

---

## Data-Centric AI/HPC Architectures

Moving data between processors and memory can dominate the cost of graph analytics, sparse computation, and modern AI inference. This research explores processing-in-memory (PIM), near-data processing, and data-movement-aware acceleration to place computation closer to data or reuse data more effectively on existing hardware. This direction also explores heterogeneous execution strategies that match workload data-access requirements with available computing and memory resources.

**Selected Publications**

- [PILOT – I/O-Aware PIM Acceleration for Long-Sequence LLM Inference with Hybrid Sparse Attention (IPDPS 2026)](../publications/IPDPS2026)
- [DynaNDE – Dynamic Near-Data Expert Scheduling for Batched MoE Inference (arXiv preprint, 2026)](https://arxiv.org/pdf/2609.00407)
- [ProMiner – Enhancing Locality, Parallelism, and Offloading for Graph Mining on Processing-in-Memory Systems (TCAD 2025)](../publications/TCAD2025)
- [CoPIM – A Concurrency-Aware PIM Workload Offloading Architecture for Graph Applications (ISLPED 2021)](../publications/ISLPED2021)

**[Complete Bibliography](/publications/)**
