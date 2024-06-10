---
title: LLM-Assisted Configuration Tuning for Log-Structured Merge-tree-based Key-Value Stores
tags: LSM-KVS, Tuning, LLM
---

Storage and Memory systems have undergone a variety of modifications and transformations, and are widely used in today's IT infrastructure. These systems usually have over 100 options (e.g. HBase and RocksDB) to tune performance for particular hardware (e.g., CPU, Memory, and Storage), software, and workloads (e.g., random, skewed, and read/write intensive). ASU-IDI focuses on developing an LLM-assisted auto-tuning framework for storage and memory systems to enhance performance.

Tuning Storage and Memory systems Log-Structured Merge-tree-based Key-Value Stores (LSM-KVS) like RocksDB and HBase with appropriate configurations is challenging, usually requiring IT professionals with appropriate expertise to run hundreds of benchmarking evaluations. Existing related studies on tuning solutions are still limited, lacking generality, adaptiveness to the versions and deployments. We believe the recent advancements of Large-Language-Models (LLMs) like OpenAI's GPT-4 can be a promising solution to achieve auto-tuning: 

1. LLMs are trained using collections of LSM-KVS-related blog, publications, and almost all the open-sourced code, which makes the LLMs a real "expert"; 
2. LLMs has the strong inferential capability to analyze the benchmarking results and achieve automatic and interactive adjustments on particular hardware and workloads. 

However, how to design the auto-tuning framework based on LLMs and benchmarking tools, how to generate appropriate prompts for LLMs, and how to calibrate the unexpected errors and wrong configurations are three main challenges to be addressed.
