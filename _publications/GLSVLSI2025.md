---
title: "Concurrency-Aware Cache Miss Cost Prediction with Perceptron Learning"
collection: publications
permalink: /publications/GLSVLSI2025
venue: "The 35th Great Lakes Symposium on VLSI (GLSVLSI 2024)"
date: 2025-6-30
---

## Abstract
The widening performance gap between processors and memory has become a major bottleneck in modern computing systems, highlighting the importance of cache performance. Traditional cache replacement policies primarily exploit data locality but often neglect the critical impact of concurrency. In fact, modern caching techniques support concurrent data accesses by servicing multiple accesses concurrently. Due to concurrency, the cost of cache misses varies significantly, offering an opportunity to enhance cache replacement by prioritizing the reduction of costly misses.

In this paper, we introduce a perceptron-based concurrency-aware miss cost predictor (CAMP) to enhance locality-based cache replacement decisions. CAMP predicts the actual cost of cache misses in environments with concurrent data accesses by analyzing multiple correlated program features. Perceptron learning is used due to its lightweight and adaptable nature, enabling accurate and generalizable predictions of cache miss costs across diverse workloads. By integrating CAMP with a locality-based cache replacement policy, we demonstrate that CAMP enhances cache management for data-intensive applications by introducing concurrency awareness. Evaluations show that integrating CAMP with SHiP++ outperforms LRU by 7.1% and 12.6% in 1-core and 4-core systems on SPEC workloads, and by 10.7% in 4-core GAP workloads, surpassing state-of-the-art policies with only modest overhead.

[paper](../files/GLSVLSI2025/GLSVLSI2025.pdf)
