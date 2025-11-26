---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: true
---

Please find my portfolio here: [pdf link](../files/portfolio.pdf).


## SimpleFSDP: Automatic Selective Unsharding for Efficient ML Systems & Distributed Training

>Research Scientist Intern at Meta Platforms – Ads Training Infra  
>Mentor: Shuai Yang | May 2025 – Aug 2025 | Sunnyvale, CA
>[Project Details Doc](https://docs.google.com/document/d/1kgBKlROezGCSbT6bxLv2RWQooqUIzo8-MSbj4euf0LQ/edit?tab=t.0)

Selective Unsharding improves FSDP throughput by strategically *retaining parameters* that reduce redundant communication. It leverages SimpleFSDP’s PT2-friendly graph structure to perform graph-level memory–communication co-optimization.
- Designed a **Selective Unsharding framework** to eliminate redundant backward all-gathers via memory-aware parameter residency.
- Built a **hierarchical PT2 graph memory profiler** mapping module ↔ graph node ↔ tensor state.
- Designed automatic greedy unshard planner (reverse-order, recursively splitting large modules, auto budget fitting).
- Added configurable all-gather bucket sizes, improving comm–compute overlap.
- Achieved **~5.5% QPS speedup** on OmniFM-v2 under 8×GPU GrandTeton.

<div style="display: flex; gap: 15px; margin-bottom: 15px;">
  <img src="/images/portfolio_images/meta_1.png" alt="Meta SimpleFSDP Selective Unsharding Figure 1" style="max-width: 60%; flex: 1;">
  <img src="/images/portfolio_images/meta_2.png" alt="Meta SimpleFSDP Selective Unsharding Figure 2" style="max-width: 40%; flex: 1;">
</div>

---

## DiT Training Simulator: Large-Scale Video Diffusion / LLM Training Simulation

>Research Scientist Intern at ByteDance – Seed (ML Systems Group)  
>Mentors: Zhihao Bai, Yanghua Peng | May 2024 – Aug 2024 | Bellevue, WA

A **perf-accurate simulator** for Diffusion Transformer (DiT) and other LLM models at 1–1000 GPU scale with multi-parallelism, timeline visualization, and memory modeling.
- Supported multiple DiT video-generation models with 95%+ forward/backward latency accuracy.
- Simulated FSDP ZeRO-2/3 with AllGather/ReduceScatter (90%+ accuracy).
- Designed full execution timeline generation → Perfetto / TensorBoard visualizations.
- Added memory profiling, tensor meta tracking, expert routing modeling.
- Extended scaling simulation to 100–1000 GPUs.
- Integrated MoE & FSDP states to **veScale** (ByteDance open-source).

---

## Out-of-GPU-Core LLM Training System (OOGC-LLM)

>Lead Researcher (with Prof. Xuehai Qian & Yikang Yue & Yuxuan Liu) | May 2023 – Jan 2024  
>Purdue University, West Lafayette, IN

A holistic rethinking of ZeRO-Offload / ZeRO-3 limitations, using multi-layer prefetching, lazy all-gather, dynamic memory management, CPU/GPU pipelining, and MoE-aware computation placement.
- Proposed multi-layer prefetching + lazy AG, reducing C2G/G2C movement.
- Designed dynamic memory manager:
  - GPU/CPU CUDA swapper  
  - CPU/NVMe swapper  
  - sliding window + priority eviction
- Built pipelined optimizer step, overlapping CPU opt with GPU fwd/bwd.
- Designed MoE optimization:  
  - hot experts → GPU, cold experts → CPU  
  - ~20% comm reduction, ~15% MoE speedup
- Delivered **≈20% end-to-end speedup** in prototype.

<div style="display: flex; gap: 15px; margin-bottom: 15px;">
  <img src="/images/portfolio_images/OOGC_1.png" alt="OOGC-LLM Architecture Figure 1" style="max-width: 48%; flex: 1;">
  <img src="/images/portfolio_images/OOGC_2.png" alt="OOGC-LLM Architecture Figure 2" style="max-width: 48%; flex: 1;">
</div>


---

## CPU Execution Engines: Inference System for ML Models on CPU

>Research Assistant (with Prof. Xuehai Qian & Gengyu Rao) | Aug 2022 – Dec 2022  
>Purdue University, West Lafayette, IN

A CPU-native depth-wise tensor execution model for efficient inference without GPU accelerators.
- Inspired by GPU tensor-grid execution; redesigned for CPU caches & NUMA.
- Implemented a tensor column depth-wise execution algorithm for better locality.
- Achieved improved CPU performance for compute-dense operators.

<img src="/images/portfolio_images/CPU_inference.png" alt="CPU Inference System Diagram" style="max-width: 65%; margin-bottom: 15px;">




---

## D-AirPatrol: Drone-based Traffic Monitoring

>MobiCom'24 Best Poster Award  
>Author (with Jiaxin Du & Prof. Chunyi Peng) | Jan 2024 – May 2024  
>Purdue University, West Lafayette, IN

Designed a drone-to-edge system for real-time vehicle detection & speed estimation.
- Built a two-layer vision system:
  - U-Net segmentation (road extraction)  
  - Motion Layer: YOLOv8 + Optical Flow + ByteTrack
- Improved tracking & reduced FP/FN using region-restricted detection.
- Evaluated across Local / Rural / Highway with **strong MOTA improvement**.
- Showed stability across altitude and resolution variations.

<div style="display: flex; gap: 15px; margin-bottom: 15px;">
  <img src="/images/portfolio_images/AirPatrol_1.png" alt="AirPatrol 1" style="max-width: 48%; flex: 1;">
  <img src="/images/portfolio_images/AirPatrol_2.png" alt="AirPatrol 2" style="max-width: 52%; flex: 1;">
</div>


---

## AirLab Platform: UAV Systems & Autonomous Drone Platforms

>Full-Stack Developer (with Jiaxin Du & Prof. Chunyi Peng)  
>Purdue University, West Lafayette, IN

A complete drone experimentation ecosystem: flight logging, DB processing, dashboard management, and map-based visualization.
- Built Android → Backend → Dashboard pipeline for image/video/flight data.
- Implemented automatic flight log parsing → MariaDB storage → map visualization.
- Developed dashboards for:
  - task, task round, flight logs  
  - drone state & user/device management  
  - field tests & check-in/out
- Designed WIP modules for labeling, training, inference.