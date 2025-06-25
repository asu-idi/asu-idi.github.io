---
title: "SHIELD: Encrypting Persistent Data of LSM-KVS from Monolithic to Disaggregated Storage" 
tags: SIGMOD, 2025
---

In this research, we introduce SHIELD, a novel log-structured-merge tree-based (e.g., RocksDB, LevelDB, and Cassandra) data encrypting, decentralized data encryption key (DEK) management, and LSM-native DEK rotation framework to address the challenges of providing robust security for high performance in both monolith and disaggregated storage deployments. 

We achieve our objective through three contributions: 
<br>
1. A fine-grained integration of encryption into LSM-KVS write path to minimize performance overhead from exposure-limiting practices like using unique encryption keys per file and regularly re-encrypting using new encryption keys during compaction, 
2. Mitigating performance degradation caused by recurring encryption of Write-Ahead Log (WAL) writes by using a buffering solution and 
3. Extending confidentiality guarantees to DS by designing a metadata-enabled encryption-key-sharing mechanism and a secure local cache for high scalability and flexibility. 
<br>
We implement both designs on RocksDB, evaluating them in monolithic and DS setups while showcasing an overhead of 0-32% for the instance-level design and 0-36% for SHIELD.

Full Paper: <a href="./../publications/files/SIGMOD25_SHIELD.pdf" target="_blank">SIGMOD25_SHIELD_Preprint.pdf</a>
<br>
GitHub URL: <a href="https://github.com/asu-idi/SHIELD" target="_blank">github.com/asu-idi/SHIELD</a>
<br>
Poster PDF: <a href="./../poster/files/SHIELD_Poster.pdf" target="_blank">SHIELD_Poster.pdf</a>

{%
  include figure.html
  image="images/posters/SHIELD_SIGMOD25_Poster.png"
  caption="The SHIELD Poster"
%}