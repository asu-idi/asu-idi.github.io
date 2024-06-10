---
title: LSM-based Key-Value Store Redesign for Disaggregated Infrastructure
tags: LSM-KVS, Disaggregation
---

LSM-KVS (e.g., RocksDB) is a key component in today’s data infrastructure for storing unstructured data. Initially designed for legacy monolithic servers, it now faces issues like resource wasting and low scalability as workloads grow. Deploying LSM-KVS in a disaggregated infrastructure is essential for better performance and resource management. Our vision is to fully restructure LSM-KVS, decouple the components, and execute them at different disaggregated compute, memory, and storage nodes for better performance, resource utilization, and management capability. Remote compaction, remote flush, and offloading the block cache are just the beginning.

Transitioning LSM-KVS-based systems to a disaggregated infrastructure involves significant changes and improvements. By decoupling the components of LSM-KVS and running them on separate compute, memory, and storage nodes, it is possible to enhance performance and scalability. This approach allows for better resource allocation, more efficient load distribution, and improved overall system management. Remote compaction, remote flush, and offloading the block cache are initial steps in this restructuring process.

- Remote Compaction: Moving the compaction process to a remote node can free up local resources, reducing bottlenecks and improving system performance.
- Remote Flush: Performing flush operations remotely can enhance data management and improve the efficiency of storage utilization.
- Offloading the Block Cache: By offloading the block cache to a remote node, it is possible to optimize memory usage and improve data retrieval times.

We envision a future where LSM-KVS is fully restructured and optimized for disaggregated infrastructure, enabling more efficient and scalable data storage solutions. By decoupling the components of LSM-KVS and distributing them across different nodes, we can address the limitations of traditional monolithic server-based systems and unlock new possibilities for data management and analysis.