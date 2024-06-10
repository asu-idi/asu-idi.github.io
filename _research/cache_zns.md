---
title: Designing and Optimizing Cache System for New Hardware and Infrastructure
tags: Cache, New-hardware, ZNS, LSM-KVS, Disaggregation, CXL, RDMA
---

Cache systems are core components of today’s data infrastructure. Our group focuses on designing and optimizing various types of cache systems for new hardware and infrastructure. Our goal is to improve the cache hit ratio, reduce costs, and achieve better management capabilities. 

Specifically, ASU-IDI is working on the following three sub-areas:

- Persistent cache optimization for Zoned Namespace SSDs: Traditionally, persistent caches have been designed based on regular SSDs, which suffer from high write amplification (i.e., shorter lifespan) and performance penalties. We aim to replace these SSDs with emerging ZNS SSDs, which can achieve larger capacity, better management capability, and almost no write amplification.
- Improving cache system performance with application hints: Historically, caches have been isolated from upper-layer applications. We are exploring various ways to use application-level information to improve the cache hit ratio and cost-effectiveness. We have investigated this with graph databases, LSM-KVS, and file systems.
- Cache in disaggregated infrastructure: With the development of memory and storage disaggregation, cache systems need to be redesigned for the new disaggregated memory (CXL-based or RDMA-based) and used to speed up disaggregated storage access. Our focus is on issues related to failure recovery, cache sharing, and cache management.