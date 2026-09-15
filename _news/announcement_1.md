---
layout: post
title: "My paper was accepted by SC'26! :sparkles: :smile:"
date: 2026-08-06 02:43:00+0800
inline: false
related_posts: false
---

### Accelerating SpGEMM Through Lightweight Clustering and Cache-Aware Accumulation

---

Sparse matrix-matrix multiplication is one of the most crucial kernels in linear algebra solvers, graph analytics, and machine learning workloads.
The clustered row-row style has emerged as a favorable SpGEMM workflow because of its potentially good parallelism.
However, due to frequent data movement caused by irregular memory access, existing approaches often suffer from three issues: (1) workload imbalance and prohibitive preprocessing overhead, (2) unsatisfactory data locality, and (3) inefficient accumulation strategy.

To this end, we propose LeSpGEMM, a **L**ocality-**e**nhanced
SpGEMM algorithm.
LeSpGEMM introduces a lightweight row-clustering method to improve spatial locality with near-linear complexity, and a cache-aware hybrid accumulation strategy to exploit data reuse across diverse sparse patterns.
It further incorporates optimized kernels, including a SIMD-accelerated dense accumulator and an efficient hash-based accumulator.
Experimental results on multiple platforms show that LeSpGEMM significantly outperforms six state-of-the-art implementations while maintaining low preprocessing overhead.

---

[LeSpGEMM Repo](https://github.com/lsl036/SparseOps)
