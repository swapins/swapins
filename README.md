# Swapin Vidya
**Systems Architect | Edge AI | ML Systems Design**

I design and build constraint-aware AI systems focused on edge deployment, reproducibility, and measurable trade-offs.

With a strong foundation in backend engineering and distributed systems, my current work focuses on:

* **Edge AI pipelines (audio and vision)**
* **Lightweight model deployment under resource constraints**
* **Reproducible ML experimentation systems**
* **Structured reasoning systems (LLM + retrieval)**

I am particularly interested in how real-world constraints—latency, memory, and reliability—shape system design decisions, especially in domains like healthcare and environmental monitoring.

By combining deterministic systems engineering with foundational medical domain knowledge and ongoing Business Administration studies, I focus on driving technical strategy and scaling decentralized AI operations for real-world infrastructure.

**All systems and prototypes presented below are designed as modular components within a unified edge-native architecture.**

---

## Flagship System — PeachbotAI

**PeachbotAI is a modular edge-native intelligence system designed for decentralized, real-time AI execution under strict resource constraints.**

It represents a **multi-layer system architecture** integrating perception, reasoning, and execution across distributed edge environments.Designed as a multi-layer system integrating perception, inference, coordination, and reasoning across distributed edge nodes.

### Core System Layers

* **Interface Layer** → Signal ingestion (audio, vision, sensor data)
* **Knowledge Layer** → Structured representations and contextual mapping
* **SBC Engine (State-Based Computation)** → Deterministic state evolution and inference
* **Decision Layer** → Constraint-aware output generation
* **FILA (Federated Intelligence Layer)** → Distributed coordination across edge nodes

### System Characteristics

* Constraint-aware execution (latency, memory, compute limits)
* Zero-cloud / privacy-aware distributed design
* Modular deployment across SBC-class hardware
* Deterministic processing pipelines for reliability

### Simplified System Flow

```text
Signals → Interface → Knowledge → SBC Engine → Decision → Local Action
                              ↓
                       Experimentation Core
                              ↓
                       Federated Layer (FILA)
```

### Engineering Focus

* Trade-offs between **accuracy vs latency vs memory**
* Deterministic vs probabilistic system behavior
* Edge-first deployment without cloud dependency
* System stability under noisy real-world inputs

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
* **Optimization:** Model quantization, deterministic edge-native execution layers

---

### Biomedical Data Systems

* Protein-protein interaction networks & TCGA dataset preprocessing
* Generic healthcare interoperability policy concepts (FHIR)
* Privacy-aware, zero-cloud distributed systems

---

## Flagship Work

### Edge-GNN Systems Analysis

**Repository:** [https://github.com/swapins/gnn-edge-systems-analysis](https://github.com/swapins/gnn-edge-systems-analysis)
**Publication:** DOI 10.5281/zenodo.19208247

A systems-level investigation into deploying Graph Neural Networks on edge hardware for biological network analysis. Instead of relying on cloud infrastructure, this deterministic system utilizes a custom **Data Structuring & Preprocessing Layer** to operate natively on resource-constrained devices.

The project explores:

* Graph Neural Network inference under strict hardware constraints
* Latency and memory behavior of deterministic GNN architectures
* Biological interaction network modeling
* Architectural strategies for hardware-aware machine learning systems

**Project Outcomes:**

* **Manuscript (Under Review):** *Edge-GNN: A Constraint-Aware Graph Neural Network Framework for Resource-Efficient Biological Interaction Modeling*
* **Patent:** Forms the architectural basis for a registered on-device clinical intelligence framework (Indian Patent No. 202541127477)

---

## System Evidence

To support architectural claims, current systems emphasize:

* Reproducible experimentation workflows (config-driven execution)
* Edge-compatible inference pipelines (CPU/SBC environments)
* Observable system behavior through logs and structured outputs
* Iterative benchmarking of latency and memory characteristics

*(Detailed benchmarks and comparative metrics are being actively expanded across systems.)*

---

## Research Identity

My research interests sit at the intersection of artificial intelligence systems, graph neural networks, and computational biology.

**Academic researcher identifier (ORCID):** 0009-0009-5758-3845

---

### Selected Publications & Manuscripts

* **Preprint:** *Edge-GNN: A Constraint-Aware Graph Neural Network Framework for Resource-Efficient Biological Interaction Modeling* (March 2026)
* **Preprint:** *Edge-Based Execution of Graph Neural Networks for Protein Interaction Network Analysis in Clinical Oncology* (January 2026)
* **Preprint:** *Dedicated Edge-AI Single-Board Computer Systems for Ecological Monitoring in Protected Wetlands* (January 2026) — under review
* **Software Publication:** *Edge-GNN Software Framework* (Zenodo DOI)

---

## Selected Architecture Prototypes

### ZeroCloud-Edge-Mesh — Distributed Edge Coordination

A **local-first, peer-to-peer coordination system** designed for running Graph Neural Network inference across distributed edge nodes without centralized infrastructure.

Focus areas include:

* Causally ordered state synchronization using Lamport clocks
* Gossip-based peer-to-peer coordination across nodes
* Deterministic local persistence using SQLite WAL
* Data-local inference for genomic sequence modeling

The system demonstrates how **edge-native biological computation can be coordinated across nodes while preserving data locality and reproducibility**, operating entirely without cloud dependency. 

---

### BioGraph-Edge-Quantizer — Resource-Aware GNN Optimization

A **quantization-aware Graph Neural Network pipeline** designed for biological interaction modeling under strict edge constraints.

Focus areas include:

* INT8 model compression (~75% footprint reduction)
* Controlled latency benchmarking under CPU-only execution
* Reproducible evaluation across x86 and ARM environments
* Trade-off analysis between accuracy and resource efficiency
  
The system highlights how **model compression impacts memory, latency, and predictive stability**, particularly in edge-constrained biological workloads. 


### Med-Guard — Edge Clinical Monitoring

A decentralized anomaly detection framework designed for **real-time physiological signal analysis on single-board computers**. Focus areas include signal normalization stability, low-latency inference, and fault-tolerant distributed monitoring architectures.

---

### Oncology-GNN-Edge — Biomedical Graph Modeling

Experimental framework for **Graph Neural Network architectures applied to protein-protein interaction networks**. Focuses on normalized graph convolution stability and the feasibility of sparse graph processing on constrained hardware platforms.

---

### Eco-Guard Ramsar — Environmental Monitoring Architecture

Experimental edge architecture combining **environmental sensor fusion with AI-assisted biological indicator detection** for distributed ecological monitoring research.

---

## Design Philosophy

Across all systems, the underlying approach is:

* Systems first, models second
* Constraints define architecture
* Determinism where reliability is critical
* Measurable trade-offs over theoretical performance

---

## Background & Education

* **Diploma in Business Administration** (In Progress)
  *Currently exploring organizations for a required short-term Corporate Attachment (Practicum) starting in August 2026, focusing on Technical Operations, Product Management, or Startup Strategy.*

* **MBBS Coursework** — Government Medical College, Thiruvananthapuram

My work integrates medical domain understanding with systems engineering to explore scalable decentralized AI architectures.

---

## Availability

Open to:

* Systems architecture roles
* Edge AI / ML systems engineering roles
* Technical strategy and operations roles
* Short-term corporate attachments (2026)

---

