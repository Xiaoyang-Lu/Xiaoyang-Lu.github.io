---
permalink: /research/
title: "Research Projects"
author_profile: true
---


## Utilizing Concurrent Data Accesses for High-Performance Data Processing

In modern computing, data-intensive applications frequently face memory bottlenecks that arise from underutilized opportunities for concurrent data access. This research investigates innovative strategies to maximize the benefits of concurrent access in cache management, offering solutions to effectively address the "Memory Wall" problem. Each study introduces specialized frameworks, metrics, and adaptive techniques designed to optimize cache performance by leveraging data access concurrency and reducing data access latency.

**Publications**

- [APAC – An Accurate and Adaptive Prefetch Framework (ICCD 2020)](../publications/ICCD2020)
- [Premier – Concurrency-Aware Cache Pseudo-Partitioning (ICCD 2021)](../publications/ICCD2021)
- [CoPIM – Concurrency-Aware PIM Architecture for Efficient Graph Offloading (ISLPED2021)](../publications/ISLPED2021)
- [CARE – Concurrency-Aware Enhanced Cache Management (HPCA 2023)](../publications/HPCA2023)
- [CHROME – Holistic Cache Management with Reinforcement Learning (HPCA 2024)](../publications/HPCA2024)
- [CAMP – Concurrency-Aware Cache Miss Cost Prediction with Perceptron Learning (GLSVLSI2025)](../publications/GLSVLSI2025)
- [ProMiner – Enhancing Locality, Parallelism, and Offloading for Graph Mining with PIM (TCAD2025)](../publications/TCAD2025)

---

## AI-Assisted Design for Performance Optimization in Computer Architecture

As modern computer systems grow in complexity and heterogeneity, traditional hardware optimization policies struggle to adapt to dynamic runtime behaviors and diverse workload demands. This research explores how AI techniques—such as reinforcement learning and lightweight perceptron models—can drive adaptive and intelligent decisions in cache and memory management, enabling systems to learn from access patterns and improve performance holistically.


**Publications**

- [CHROME – Holistic Cache Management with Reinforcement Learning (HPCA2024)](../publications/HPCA2024)
- [CAMP – Concurrency-Aware Cache Miss Cost Prediction with Perceptron Learning (GLSVLSI2025)](../publications/GLSVLSI2025)
- [COSMOS - Counter Cache Optimization for Secure Memory with Reinforcement Learning (MICRO2025)](../publications/MICRO2025)

---



## Efficient Hardware Design for AI Computing

As AI applications grow in complexity, they demand increasingly efficient hardware architectures to manage huge memory demands and high-dimensional computations. This research focuses on designing hardware solutions that not only accelerate AI computation but also optimize memory access efficiency—a critical factor in achieving high performance in data-intensive AI tasks.

**Publications**

- [ACES – Adaptive and Concurrency-Aware Sparse Matrix Accelerator (ASPLOS2024)](../publications/ASPLOS2024)
- [Pyramid – Accelerating LLM Inference with PIM (CAL2025)](../publications/CAL2025)
- [Zion – A Comprehensive, Adaptive, and Lightweight Hardware Prefetcher (DATE2026)](../publications/DATE2026)
- [AttenIO – An I/O Analysis for Long-Sequence Attention (ASPLOS2026)](../publications/ASPLOS2026)
- [PILOT – I/O-Aware PIM Acceleration for Long-Sequence LLM Inference with Hybrid Sparse Attention (IPDPS2026)](../publications/IPDPS2026)

---

## Leveraging Processing-in-Memory for Data-Intensive Applications

Data-intensive applications, particularly those involving complex graph computations, face significant performance bottlenecks due to heavy data movement and irregular memory access patterns. This research explores innovative processing-in-memory (PIM) architectures to tackle these challenges, reducing the reliance on CPU and minimizing data transfer overhead. Each study introduces a unique approach to enhance graph computing efficiency through PIM by leveraging memory locality and concurrency.

**Publications**

- [CoPIM – Concurrency-Aware PIM Architecture for Efficient Graph Offloading (ISLPED2021)](../publications/ISLPED2021)
- [AceMiner – Accelerating Graph Pattern Matching with In-DRAM Caching (ICCD2024))](../publications/ICCD2024)
- [ProMiner – Enhancing Locality, Parallelism, and Offloading for Graph Mining with PIM (TCAD2025)](../publications/TCAD2025)
- [PILOT – I/O-Aware PIM Acceleration for Long-Sequence LLM Inference with Hybrid Sparse Attention (IPDPS2026)](../publications/IPDPS2026)

---

## Concurrency-Aware Memory Performance Modeling

Driven by the demands of big data applications and high-performance computing, modern computing requires precise memory performance models that effectively capture the impact of concurrency. This research delves into how concurrent data access influences memory system performance, introducing advanced modeling techniques to deepen our understanding of memory bottlenecks, particularly within multi-core systems where concurrency is a critical factor.


**Publications**

- [A Generalized Model for Modern Hierarchical Memory Systems (WSC2022)](../publications/WSC2022)
- [The Memory-Bounded Speedup Model and Its Impacts in Computing (JCST2023)](../publications/JCST2023)


---

## I/O Analysis: Building an Analytical Foundation for Data-Centric Computing

Unbalanced technological progress between processors and memory has led to the persistent “memory wall”, fundamentally constraining the performance of modern computing systems. At the same time, the rapid growth of memory-intensive workloads such as machine learning, graph processing, and scientific data analysis has produced massive datasets and significantly increased demands on data movement across memory hierarchies, making system performance more frequently limited by data movement (I/O) than by arithmetic computation. While computational complexity analysis has long guided algorithm design in compute-centric systems, it does not capture the fundamental cost of data movement across memory systems. This gap motivates the need for a principled I/O complexity analysis framework for data-centric system design, where input/output broadly denotes data access and movement across memory levels. This project argues that I/O complexity analysis plays a role in data-centric architectures comparable to that of arithmetic complexity in compute-centric design, and accordingly develops new I/O analysis frameworks, establishes I/O lower-bound reasoning, and introduces constructive methods to translate algorithm-inherent I/O bounds into actionable execution strategies and architecture design decisions.


**Publications**

- [AttenIO – An I/O Analysis for Long-Sequence Attention (ASPLOS2026)](../publications/ASPLOS2026)
- [PILOT – I/O-Aware PIM Acceleration for Long-Sequence LLM Inference with Hybrid Sparse Attention (IPDPS2026)](../publications/IPDPS2026)
