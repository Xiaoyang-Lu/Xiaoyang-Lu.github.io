---
title: "Research Projects"
permalink: /research/
author_profile: true
---

## Utilizing Concurrent Data Accesses for High-Performance Data Processing

In modern computing, data-intensive applications often encounter memory bottlenecks due to unutilized concurrency in data access. This research explores various strategies to fully harness concurrent data access capabilities within cache management systems, addressing the memory wall problem effectively. Each project introduces unique frameworks, metrics, and adaptive mechanisms to optimize cache performance through enhanced memory parallelism.

## Projects:

- [APAC – An Accurate and Adaptive Prefetch Framework](#apac-an-accurate-and-adaptive-prefetch-framework)
- [CARE – Concurrency-Aware Enhanced Cache Management](#care-concurrency-aware-enhanced-cache-management)
- [Premier – Concurrency-Aware Cache Pseudo-Partitioning](#premier-concurrency-aware-cache-pseudo-partitioning)
- [CHROME – Holistic Cache Management with Reinforcement Learning](#chrome-holistic-cache-management-with-reinforcement-learning)

Each project’s detailed exploration includes background, motivation, features, results, and a conclusion, providing insights into their contributions to enhancing memory concurrency and reducing cache misses.

---

### APAC: An Accurate and Adaptive Prefetch Framework

**Background**:  
The "Memory Wall" remains a persistent problem as processor speeds outpace memory access rates, leading to significant stalls in data-intensive applications. Traditional prefetching methods are effective to some extent but fail to fully address concurrent memory access scenarios, where multiple overlapping requests impact performance unpredictably.

**Motivation**:  
APAC was developed to introduce Pure Prefetch Coverage (PPC), a metric that enhances traditional prefetching by considering concurrent memory access. This new metric helps gauge the real effectiveness of prefetching in systems where data concurrency is high, enabling more accurate and adaptable prefetching strategies.

**Key Features**:
- **Pure Prefetch Coverage (PPC)**: Improves on the conventional Prefetch Coverage metric by capturing the impact of concurrent accesses, allowing for precise adjustments in prefetching aggressiveness.
- **Adaptive Prefetch Tuning**: By dynamically monitoring PPC and Pure Miss Rate (pMR), APAC adapts its prefetching intensity to maintain optimal cache utilization under varying memory access conditions.

**Results**:  
APAC demonstrates significant improvements in both single-threaded and multi-core environments, with an average 17.3% IPC gain in single-thread memory-intensive benchmarks and an 8.5% IPC gain in multi-core systems.

**Conclusion**:  
APAC’s adaptive approach to prefetching shows that accurately measuring and leveraging concurrency in memory access can result in significant performance gains, making it a robust solution for data-intensive applications.

**Publication**: [ICCD2020: APAC Paper](../publications/ICCD2020_APAC)

---

### CARE: Concurrency-Aware Enhanced Cache Management

**Background**:  
Cache performance is traditionally optimized by focusing on data locality, but with the rise of multi-core systems, there is a need to consider data access concurrency to handle the increased demand effectively. CARE addresses this by introducing a concurrency-aware approach.

**Motivation**:  
CARE was created to improve on standard cache management by accounting for concurrent data access patterns. Through the Pure Miss Contribution (PMC) metric, CARE quantifies the cost of cache misses, optimizing cache replacement decisions with both locality and concurrency in mind.

**Key Features**:
- **Pure Miss Contribution (PMC)**: This metric measures the relative performance impact of each outstanding cache miss, enabling cache replacement decisions that prioritize high-impact misses.
- **Dynamic Threshold Reconfiguration Mechanism (DTRM)**: CARE’s DTRM adapts cache management dynamically based on PMC and application phase, making it a flexible solution across diverse workloads.

**Results**:  
CARE outperforms LRU replacement policies, achieving a 10.3% IPC improvement in 4-core systems, and up to 17.1% in 16-core systems, showcasing its scalability in high-concurrency environments.

**Conclusion**:  
CARE illustrates that by integrating concurrency-aware metrics, cache management frameworks can significantly improve cache efficiency, especially in multi-core setups with high concurrent data demands.

**Publication**: [HPCA2023: CARE Paper](../publications/HPCA2023_CARE)

---

### Premier: Concurrency-Aware Cache Pseudo-Partitioning Framework

**Background**:  
As multi-core processors handle increasingly complex applications, shared last-level caches (LLCs) experience contention, leading to performance degradation. Cache partitioning can mitigate this by controlling cache allocations per core but often overlooks concurrency.

**Motivation**:  
Premier leverages Pure Misses Per Kilo Instructions (PMPKI), a concurrency-aware metric that optimizes cache partitioning decisions by assessing the real cost of cache misses under concurrent access. By focusing on pure misses rather than total misses, Premier improves both performance and fairness across workloads.

**Key Features**:
- **Pure Misses Per Kilo Instructions (PMPKI)**: Assesses cache miss impact in concurrent access scenarios, providing an effective indicator for partitioning decisions.
- **Dynamic Cache Allocation**: Using PMPKI curves, Premier adapts cache allocation in real-time, balancing between performance and fairness for each application in multi-core setups.

**Results**:  
Premier outperforms traditional partitioning schemes, achieving a 15.45% performance improvement and a 10.91% fairness increase in 8-core systems, demonstrating its strength in managing shared LLC resources effectively.

**Conclusion**:  
Premier’s concurrency-aware approach to cache partitioning highlights the importance of pure misses in optimizing cache efficiency, especially in scenarios with high core counts and shared resources.

**Publication**: [ICCD2021: Premier Paper](../publications/ICCD2021_Premier)

---

### CHROME: Holistic Cache Management with Reinforcement Learning

**Background**:  
As data-intensive workloads continue to grow, cache management techniques—such as replacement, bypassing, and prefetching—are essential but are often treated independently. CHROME integrates these techniques using an online reinforcement learning framework to achieve a cohesive cache management strategy.

**Motivation**:  
CHROME aims to bridge the gap between separate cache management techniques by leveraging reinforcement learning to optimize cache actions dynamically. By monitoring both data locality and concurrency, CHROME adapts to diverse workloads and system configurations in real time.

**Key Features**:
- **Holistic Cache Management**: Combines cache replacement, bypassing, and prefetching to optimize cache usage.
- **Online Reinforcement Learning**: Employs reinforcement learning to continually adjust cache decisions based on observed workload characteristics, improving adaptability.
- **Concurrency-Aware System Feedback**: Provides CHROME with system-level feedback, enhancing its ability to make accurate cache management decisions.

**Results**:  
CHROME outperforms existing cache management schemes, achieving a 13.7% performance improvement over the LRU baseline in 16-core systems and consistently surpassing competing frameworks in diverse workloads.

**Conclusion**:  
CHROME’s holistic and adaptive approach demonstrates the benefits of combining multiple cache management strategies through reinforcement learning, underscoring its potential as a versatile solution for high-performance computing systems.

**Publication**: [HPCA2024: CHROME Paper](../publications/HPCA2024_CHROME)

---

## Final Summary

Each project in this research initiative tackles specific challenges within cache management by integrating concurrency-aware metrics and adaptive frameworks. Collectively, they demonstrate the significant performance improvements possible by strategically managing concurrent memory accesses, helping overcome the memory wall problem that plagues data-intensive applications in multi-core environments.
