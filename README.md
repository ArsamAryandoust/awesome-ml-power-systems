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

Only research articles with publicly available source code are included in this collection. Articles whose reported results cannot be independently reproduced are removed as reproducibility assessments become available.

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
- [Datasets](#datasets)
- [Open-Source Software](#open-source-software)
- [Open Research Challenges](#open-research-challenges)
- [Contributing](#contributing)

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

| Area | Survey | Venue | Year |
|--------|--------|--------|--------|
| Application overview | [Tackling Climate Change with Machine Learning](https://dl.acm.org/doi/10.1145/3485128) | ACM Computing Surveys | 2022 |
| Physics-Informed Learning | [Physics-informed machine learning](https://www.nature.com/articles/s42254-021-00314-5) | Nature Reviews Physics | 2021 |

---

## Recommended Tutorials

| Area | Survey | Venue | Year |
|--------|--------|--------|--------|
| ML for Optimization | [Tutorial on amortized optimization](https://arxiv.org/abs/2202.00665) | Foundations and Trens in Machine Learning | 2025 |
| Enforcing constraints | [Deep Implicit Layers - Neural ODEs, Deep Equilibirum Models, and Beyond](https://implicit-layers-tutorial.org) | NeurIPS | 2020 |

---

## Recommended Textbooks

| Area | Textbook | Year |
|--------|--------|--------|
| Machine Learning | [Probabilistic Machine Learning: An Introduction](https://probml.github.io/pml-book/book1.html) | 2022 |
| Geometric Deep Learning | [Geometric Deep Learning: Grids, Groups, Graphs, Geodesics, and Gauges](https://geometricdeeplearning.com) | 2024 |
| Reinforcement Learning | [Reinforcement Learning and Optimal Control](http://www.athenasc.com/index.html) | 2019 |
| Reinforcement Learning | [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book-2nd.html) | 2018 |

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

### Papers

| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| TBD | | | |

---

## Simulation

Applications include:

- Power Flow (PF) simulations
- Electro Magnetic Transient (EMT) simulations 


### Papers

| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| TBD | | | |

---

## Optimization

Applications include:

- AC optimal power flow (ACOPF)
- Unit Commitment
- Security-constrained ACOPF


### Papers

| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| TBD | | | |

---

## Control

Applications include:

- Voltage control
- Frequency control
- Demand response
- Topology switching
- Converter control


### Papers

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


### Papers

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

### Papers

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


### Papers

| Year | Venue | Title | Task |
|--------|--------|--------|-------- |
| TBD | | | |

---

# Datasets

## Standardized Collections

| Dataset | Description |
|----------|-------------|
| [AI.grids v1](https://huggingface.co/AI-grids) | A growing collection of standardized machine-learning datasets for power-system applications, including electricity consumption, renewable energy, and grid-related benchmarks designed to facilitate reproducible ML research.|

---

## ACOPF

| Dataset | Description |
|----------|-------------|
| [OPFData](https://arxiv.org/abs/2406.07234) | Large-scale open dataset for AC Optimal Power Flow (ACOPF) containing solved OPF instances with realistic topological perturbations. Developed to support data-driven OPF research and scalable machine-learning approaches for power-system optimization.|


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

## Machine Learning

| Tool | Description |
|--------|-------------|
| PyTorch | Deep learning framework |
| JAX | High-performance ML framework |


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

# Contributing

Contributions are welcome.

Please submit a pull request to:

- Add missing papers
- Add datasets
- Add software tools
- Correct metadata
- Improve categorization


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
