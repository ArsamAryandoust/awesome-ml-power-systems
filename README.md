# Awesome Machine Learning for Power Systems
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated collection of papers, datasets, software, benchmarks, and resources at the intersection of machine learning and electric power systems.

This repository aims to provide researchers, students, and practitioners with a structured overview of the rapidly growing field of machine learning for electric power systems.

Unlike other paper lists, this repository emphasizes:
- Research categorization
- Reproducibility (code availability)
- Datasets and benchmarks
- Open-source tools
- Research gaps and future directions

Only research articles with publicly available source code and datasets are included in this collection. Articles whose reported results cannot be independently reproduced are removed as reproducibility assessments become available.

---

## Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Research Areas](#research-areas)
  - [Forecasting](#forecasting)
  - [Simulation](#simulation)
  - [Optimization](#optimization)
  - [Control](#control)
  - [Neural Network Architectures](#neural-network-architectures)
  - [Electricity Markets](#electricity-markets)
  - [Foundation Models & LLMs](#foundation-models--llms)
  - [Miscellaneous](#miscellaneous)
- [Open-Source Software](#open-source-software)
- [Open Research Challenges](#open-research-challenges)

---

# Introduction

Electric power systems are undergoing a profound transformation driven by:

- Renewable energy integration
- Electrification of transportation and heating
- Distributed energy resources
- Increased uncertainty in system operation
- Growing computational complexity

At the same time, machine learning has experienced rapid advances in:

- Deep learning
- Reinforcement learning
- Graph neural networks
- Generative AI
- Foundation models
- Scientific machine learning

This repository tracks research at the intersection of these two fields. Electrifying energy consumption and meeting that demand with renewable energy sources is a central strategy for mitigating global warming and climate change. This shared objective motivates much of the research conducted at this intersection.

---

# Getting Started



## Recommended Surveys

| Area | Title | Venue | Year |
|--------|--------|--------|--------|
| Application overview | [Tackling Climate Change with Machine Learning](https://dl.acm.org/doi/10.1145/3485128) | ACM Computing Surveys | 2022 |
| Physics-Informed Learning | [Physics-informed machine learning](https://www.nature.com/articles/s42254-021-00314-5) | Nature Reviews Physics | 2021 |

---

## Recommended Tutorials

| Area | Title | Venue | Year |
|--------|--------|--------|--------|
| ML for Optimization | [Tutorial on amortized optimization](https://arxiv.org/abs/2202.00665) | Foundations and Trens in Machine Learning | 2025 |
| Enforcing constraints | [Deep Implicit Layers - Neural ODEs, Deep Equilibirum Models, and Beyond](https://implicit-layers-tutorial.org) | NeurIPS | 2020 |

---

## Recommended Textbooks

| Area | Title | Year |
|--------|--------|--------|
| Machine Learning | [Probabilistic Machine Learning: An Introduction](https://probml.github.io/pml-book/book1.html) | 2022 |
| Geometric Deep Learning | [Geometric Deep Learning: Grids, Groups, Graphs, Geodesics, and Gauges](https://geometricdeeplearning.com) | 2024 |
| Reinforcement Learning | [Reinforcement Learning and Optimal Control](http://www.athenasc.com/index.html) | 2019 |
| Reinforcement Learning | [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book-2nd.html) | 2018 |

---

## Recommended Lectures

| Title | Lecturer |
|--------|-------------|
| [MIT 6.S191 Introduction to Deep Learning](https://introtodeeplearning.com) | Alexander and Ava Amini |
| [Stanford CS224W Machine Learning with Graphs](https://www.youtube.com/watch?v=JAB_plj2rbA&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn) | Jure Leskovec |


---

## Recommended ML Frameworks & Tools

| Tool | Description |
|--------|-------------|
| [PyTorch](https://pytorch.org) | Deep learning framework |
| [JAX](https://docs.jax.dev/en/latest/) | High-performance ML framework |
| [WandB](https://wandb.ai/site/) | MLOps for tracking, visualizing and optimizing models |


---

# Research Areas

We distinguish the following research areas:

- [Forecasting](#forecasting)
- [Simulation](#simulation)
- [Optimization](#optimization)
- [Control](#control)
- [Neural Network Architectures](#neural-network-architectures)
- [Electricity Markets](#electricity-markets)
- [Foundation Models & LLMs](#foundation-models--llms)


## Forecasting

Applications include:

- Load forecasting
- Solar forecasting
- Wind forecasting
- Hydro forecasting
- Fault forecasting


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| 2024 | NeurIPS (Datasets & Benchmarks) | [PowerGraph: A Power Grid Benchmark Dataset for Graph Neural Networks](https://proceedings.neurips.cc/paper_files/paper/2024/hash/c7caf017cbbca1f4b368ffdc7bb8f319-Abstract-Datasets_and_Benchmarks_Track.html) | Cascading failure forecasts based on grid state |
| 2024 | Energy \& Buildings | [Benchmarking reservoir computing for residential energy demand forecasting](https://www.sciencedirect.com/science/article/pii/S0378778824003529) | Autoregressive electric load forecasting |
| 2022 | Nature Machine Intelligence | [Enhanced spatio-temporal electric load forecasts using less data with active deep learning](https://www.nature.com/articles/s42256-022-00552-x) | Spatial electric load forecasting |

---

## Simulation

Applications include:

- Power Flow (PF) simulations
- Electro Magnetic Transient (EMT) simulations 


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| 2025 | ICML | [Optimization Proxies using Limited Labeled Data and Training Time: A Semi-Supervised Bayesian Neural Network Approach](https://openreview.net/forum?id=Jnpgx8OzfD) | Learning surrogates/proxies for power-flow and power-system optimization |
| 2025 | NeurIPS (Datasets & Benchmarks) | [PFΔ: A Benchmark Dataset for Power Flow under Load, Generation, and Topology Variations](https://openreview.net/forum?id=Gi1HtsTAkv) | Benchmarking machine-learning methods for power-flow prediction and analysis |

---


## Optimization

Applications include:

- AC optimal power flow (ACOPF)
- Unit Commitment
- Security-constrained ACOPF


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| 2024 | ICML | [Compact Optimality Verification for Optimization Proxies](https://dl.acm.org/doi/10.5555/3692070.3692378) | Structuring a gradient-based primal heuristic formulation to verify and bound worst-case optimality gaps for DC-OPF neural network proxies. |
| 2024 | Google DeepMind | [OPFData: Large-scale datasets for AC optimal power flow with topological perturbations](https://arxiv.org/abs/2406.07234) | Large collection of solved instances for ACOPF with ten grid topologies |
| 2023 | ICML | [Low Complexity Homeomorphic Projection to Ensure Neural-Network Solution Feasibility for Optimization over (Non-)Convex Set](https://proceedings.mlr.press/v202/liang23a.html) | Feasibility projection for neural-network solutions to AC optimal power flow (AC-OPF) |
| 2021 | NeurIPS | [Adversarially Robust Learning for Security-Constrained Optimal Power Flow](https://proceedings.neurips.cc/paper/2021/hash/f0f07e680de407b0f12abf15bd520097-Abstract.html) | Learning-based optimization for security-constrained OPF under adversarial uncertainty |




---

## Control

Applications include:

- Voltage control
- Frequency control
- Demand response
- Topology switching
- Converter control


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| TBD | | | |

---

## Neural Network architectures

Applications include:

- graph neural networks
- geometric deep learning architectures
- physics-informed architectures
- neuro-symbolic architectures


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| TBD | | | |

---

## Electricity Markets

Applications include:

- Price forecasting
- Bidding strategies
- Market simulation
- Market design


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| TBD | | | |

---

## Foundation Models & LLMs

Applications include:

- Multi-modal, multi-tasking ML for power systems tasks
- Grid operation assistants
- Power-system copilots
- Retrieval-augmented systems
- Domain-specific foundation models


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| 2026 | Hugging Face | [AI.grids v1](https://huggingface.co/AI-grids) | A growing collection of standardized machine-learning datasets for power-system applications, including electricity consumption, renewable energy, and grid-related benchmarks designed to facilitate reproducible ML research.|
| 2024 | NeurIPS | [PowerPM: Foundation Model for Power Systems](https://proceedings.neurips.cc/paper_files/paper/2024/hash/d0a2279c9f7ded859bcbf878c3c3d1ed-Abstract-Conference.html) | Foundation model / representation learning for power-system tasks |

---



## Miscellaneous

Applications include:

- Physics-informed benchmarking


| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| 2022 | NeurIPS | [LIPS - Learning Industrial Physical Simulation benchmark suite](https://proceedings.neurips.cc/paper_files/paper/2022/hash/b3ac9866f6333beaa7d38926101b7e1c-Abstract-Datasets_and_Benchmarks.html) | A modular benchmark suite for evaluating data-driven augmented physical simulators on industrial use cases, such as power grids and pneumatics, across criteria including accuracy, efficiency, robustness, and real-world applicability.|

---

# Open-Source Software

## Power Systems

| Tool | Description |
|--------|-------------|
| pandapower | Open-source power-system analysis framework |
| PyPSA | Python for Power System Analysis |
| MATPOWER | Power flow and optimization toolkit |

---

## Reinforcement Learning

| Tool | Description |
|--------|-------------|
| Grid2Op | Benchmark platform for power-grid operation |
| PowerGridworld | RL environments for power systems |

---

# Open Research Challenges

The following research challenges remain largely open.

## Reliable Deployment

Many methods perform well in simulation but remain difficult to deploy in real-world power systems.

## Benchmarking

The community lacks widely accepted benchmarks and evaluation protocols.

## Generalization

Models often struggle under changing operating conditions.

## Safety and Trustworthiness

Power-system operators require interpretable, robust, and reliable models.

## Foundation Models for Power Systems

The role of large-scale pretrained models remains largely unexplored.

## Offline Reinforcement Learning

Safe learning from historical operational data remains a major challenge.

---

# Future Trends

Potential high-impact research directions include:

- Foundation models for grid operation
- Multi-agent energy systems
- AI agents for system operation
- Physics-informed generative models
- Foundation datasets for power systems
- Reliable uncertainty quantification
- Human-AI collaboration in control rooms
- Explainable and interpretable AI for power systems
- Neurosymbolic models for power systems

---

# Citation

If you find this repository useful, please consider starring it and citing it.

```bibtex
@misc{aryandoust2026awesome,
  author = {Aryandoust, Arsam},
  title = {Awesome Machine Learning for Power Systems},
  year = {2026},
  publisher = {GitHub},
  howpublished = {\url{https://github.com/ArsamAryandoust/awesome-ml-power-systems}}
}
```

---
