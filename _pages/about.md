---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a fourth-year Ph.D student advised by [Prof. Chunyi Peng](https://www.cs.purdue.edu/homes/chunyi/) in Computer Science at Purdue University. Before that, I was advised by [Prof. Xuehai Qian](https://hpc.cs.tsinghua.edu.cn/en/info/1537/2730.htm) in Computer Science at Purdue University for one and a half years. Before joining Purdue, I received my B.E. degree in 2022 from Department of Automation, Tsinghua University.

My research interests are in the field of machine learning systems especially in LLMs and agentic drones. I'm specializing in large-scale machine learning systems, LLM infrastructure, and efficient training/inference pipelines. My work spans distributed training (FSDP, ZeRO, Megatron), GPU/CPU memory–computation optimization, and large-cluster LLM simulation, strengthened through research roles at ByteDance and Meta. In parallel, I develop end-to-end embodied AI systems, including award-winning drone-based perception platforms that integrate real-time vision, optimization, and robotics. I am committed to advancing scalable AI systems and next-generation intelligent agents.


## News
- [5/2025] Started Research Scientist internship at Meta Platforms – Ads Training Infra, Sunnyvale, CA, working on Distributed ML Systems.
- [11/20/2024] Jiaxin Du and I received MobiCom 2024 Best Poster Award.
- [11/1/2024] Our short paper "D-AirPatrol: A Dual-Layer Architecture for Traffic Patrol From the Sky" has been accepted by MobiCom'24.
- [5/2024] Started Research Scientist internship at ByteDance – Seed, Bellevue, WA, working on LLM Infrastructure.
- 
## Experience

- Meta Platforms – Ads Training Infra, Sunnyvale, CA  
  Research Scientist Intern in Distributed ML Systems (Mentor: Shuai Yang), May 2025 – Aug 2025  
  - Collaborated with the FAIR PyTorch/FSDP team to co-design and implement an Automatic Selective Unsharding framework atop SimpleFSDP (a PyTorch 2.0 compile-friendly FSDP), improving communication–computation overlap and training efficiency.  
  - Built a hierarchical memory profiler and adaptive unsharding algorithm leveraging GPU memory budget for selective parameter retention, achieving up to 5.5% QPS improvement on 8×GPU ads-model benchmarks.  
  - Enhanced SimpleFSDP infrastructure with configurable communication scheduling and integrated memory–computation optimization, enabling future adaptive distributed-training pipelines within Meta Ads Infra.

- ByteDance – Seed, Bellevue, WA  
  Research Scientist Intern in LLM Infrastructure (Mentor: Yanghua Peng), May 2024 – Sep 2024  
  - Supported an LLM training simulator to profile and simulate the training latency of LLMs (especially diffusion transformer models) on 1k–10k GPUs for text-to-video generation and customized computing kernels to achieve 95%+ accuracy.  
  - Supported memory profiling and distributed training simulation in frameworks like `torch.distributed` and DeepSpeed-Megatron within the LLM training simulator and achieved 95% accuracy.  
  - Supported PyTorch FSDP and various parallelism techniques in ByteDance’s open-source distributed training stack.

- Purdue University
  - Teaching Assistant
    - CSCI 48700 Artificial Intelligence (2025 Fall)
    - CS 18200 Foundations Of Computer Science (2025 Spring)
    - CS 25000 Computer Architecture  (2024 Spring)
    - CS 53600 Data Communication and Computer Networks  (2023 Fall & 2024 Fall)
  - Research Assistant in Dr. Xuehai Qian's Lab  (Aug 2022 - Sep 2023)

## Portfolio
Please go to the portfolio page: [Portfolio](/portfolio/)
Please find my portfolio here: [pdf link](../files/portfolio.pdf).

## Awards
- MobiCom'24 Best Poster Award;   _Oct 2024_
- Technological Innovation Scholarship of Tsinghua University;   _Oct 2021_
- 2019 & 2020 Hage Foundation Scholarship;   _Apr 2019 & Apr 2020_
- AI Competition of Tsinghua University Third Award;  _Jun 2021_
- Winning Prize of Electronics Design Contest of Tsinghua University  _Aug 2020_
