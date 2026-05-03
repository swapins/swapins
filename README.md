# Swapin Vidya

**Systems Architect | Edge AI | ML Systems Design**

I design and build **constraint-aware AI systems** focused on edge deployment, reproducibility, and measurable trade-offs.

With a strong foundation in backend engineering and distributed systems, my current work focuses on:

* **Edge AI pipelines (audio and vision)**
* **Lightweight model deployment under resource constraints**
* **Reproducible ML experimentation systems**
* **Structured reasoning systems (LLM + retrieval)**

I am particularly interested in how **real-world constraints—latency, memory, and reliability—shape system design decisions**, especially in domains like healthcare and environmental monitoring.

By combining deterministic systems engineering with foundational medical domain knowledge and ongoing Business Administration studies, I focus on **designing and evaluating decentralized AI systems for real-world infrastructure**.

---

```text
All systems and prototypes presented below are designed as modular components within a unified edge-native architecture.
```

---

## Flagship System — PeachbotAI

**PeachbotAI is a modular edge-native intelligence system designed for decentralized, real-time AI execution under resource constraints.**

Designed as a **multi-layer system integrating perception, inference, coordination, and reasoning across distributed edge nodes.**

> ⚠️ **Scope:** This is an actively evolving prototype system focused on architecture validation and constraint-driven experimentation, not a production deployment.

---

### Core System Layers

* **Interface Layer** → Signal ingestion (audio, vision, sensor data)
* **Knowledge Layer** → Structured representations and contextual mapping
* **SBC Engine (State-Based Computation)** →
  *Deterministic execution pipeline (state-machine style processing; reproducible given fixed inputs and weights)*
* **Decision Layer** → Constraint-aware output generation
* **FILA (Federated Intelligence Layer)** →
  *Lightweight coordination layer (gossip-style synchronization + eventual consistency concepts)*

---

### System Characteristics

* Constraint-aware execution (latency, memory, compute limits)
* Edge-first design (cloud optional, not required for inference)
* Modular deployment across SBC-class hardware
* Reproducible execution pipelines (fixed seeds, deterministic flow control)

---

### Simplified System Flow

```text
Signals → Interface → Knowledge → SBC Engine → Decision → Local Action
                              ↓
                       Experimentation Core
                              ↓
                       Federated Layer (FILA)
```

---

### Engineering Focus

* Trade-offs between **accuracy vs latency vs memory**
* Deterministic execution vs probabilistic model outputs
* Edge-first deployment under CPU/SBC constraints
* Stability under noisy real-world inputs

---

### Example Execution Context

* Device: Intel i5-class CPU / Raspberry Pi-class SBC
* Execution Mode: CPU-only
* Pipeline: signal → preprocessing → model inference → structured output
* Latency (prototype range): ~100–300 ms depending on model size
* Memory footprint: optimized via quantization and bounded model size

*(Benchmarks are being standardized across systems for consistency.)*

---

## Technical Stack

### Systems Architecture & Infrastructure

* **Backend:** PHP (Senior), Laravel, PostgreSQL / MySQL, Redis
* **Distributed Systems:** Docker, Kubernetes, Linux systems administration
* **Architecture:** RESTful and GraphQL APIs, MQTT messaging systems, Event-driven microservices

---

### Machine Learning & Edge Systems

* **Frameworks:** PyTorch, TensorFlow Lite, Graph Neural Networks (GNNs)
* **Hardware:** NVIDIA Jetson, SBC-class hardware, low-latency execution
* **Optimization:** Model quantization, resource-aware inference pipelines

---

### Biomedical Data Systems

* Protein-protein interaction networks & TCGA dataset preprocessing
* Healthcare interoperability concepts (FHIR — structural alignment only)
* Privacy-aware, decentralized system design

---

## Flagship Work

### Edge-GNN Systems Analysis

**Repository:** [https://github.com/swapins/gnn-edge-systems-analysis](https://github.com/swapins/gnn-edge-systems-analysis)
**Publication:** DOI 10.5281/zenodo.19208247

A systems-level investigation into deploying Graph Neural Networks on edge hardware for biological network analysis.

Focus areas:

* GNN inference under hardware constraints
* Latency and memory trade-offs
* Biological interaction modeling
* Architecture patterns for edge ML systems

**Project Outcomes:**

* Manuscript under review
* Patent (filed; not yet granted)

---

## System Evidence

To support architectural claims, current systems emphasize:

* Reproducible experimentation workflows (config-driven execution)
* Edge-compatible inference pipelines (CPU/SBC environments)
* Observable behavior through logs and structured outputs
* Iterative benchmarking of latency and memory characteristics

---

## Research Identity

My research interests sit at the intersection of artificial intelligence systems, graph neural networks, and computational biology.

**ORCID:** 0009-0009-5758-3845

---

## Selected Architecture Prototypes

### ZeroCloud-Edge-Mesh — Distributed Edge Coordination

A **local-first coordination prototype** for synchronizing edge nodes running GNN inference.

* Gossip-style synchronization
* Lamport-clock-based ordering
* SQLite WAL persistence
* Designed for data-local execution

---

### BioGraph-Edge-Quantizer — Resource-Aware GNN Optimization

A **quantization-aware GNN pipeline** for biological interaction modeling under edge constraints.

* ~75% model size reduction via INT8
* <1% accuracy degradation observed
* CPU and ARM execution tested
* Focus: memory vs accuracy trade-offs

---

### Med-Guard — Edge Clinical Monitoring

A decentralized anomaly detection framework for **real-time physiological signal analysis** on SBC devices.

---

### Oncology-GNN-Edge — Biomedical Graph Modeling

Experimental framework for **GNN-based protein interaction modeling** under constrained compute environments.

---

### Eco-Guard Ramsar — Environmental Monitoring Architecture

Edge-based system combining **sensor fusion and AI-assisted ecological detection**.

---

## Design Philosophy

* Systems first, models second
* Constraints define architecture
* Deterministic execution for reproducibility
* Measurable trade-offs over theoretical performance

---

## Background & Education

* Diploma in Business Administration (In Progress)
* MBBS Coursework — Government Medical College

---

## Availability

Open to:

* Systems architecture roles
* Edge AI / ML systems engineering roles
* Technical strategy and operations roles
* Corporate attachments (2026)

---
