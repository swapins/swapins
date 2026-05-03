# Swapin Vidya

**Systems Architect | Edge AI | ML Systems Design**

**Primary focus: Edge-constrained ML systems (with emphasis on GNN workloads and structured data pipelines).**

I design and build **constraint-aware AI systems** focused on edge deployment, reproducibility, and measurable trade-offs.

With a strong foundation in backend engineering and distributed systems, my current work focuses on:

* **Edge AI pipelines (audio and vision)**
* **Lightweight model deployment under resource constraints**
* **Reproducible ML experimentation systems**
* **Structured reasoning pipelines (LLM-assisted retrieval, experimental)**

I am particularly interested in how **real-world constraints—latency, memory, and reliability—shape system design decisions**, especially in domains like healthcare and environmental monitoring.

By combining systems engineering with foundational medical domain knowledge and ongoing Business Administration studies, I focus on **designing and evaluating decentralized AI systems for real-world infrastructure**.

---

```text
All systems and prototypes presented below are designed as modular components within a unified edge-native architecture.
```

---

## Flagship System — PeachbotAI

**PeachbotAI is a modular edge-native system designed to explore decentralized, real-time AI execution under resource constraints.**

Designed as a **multi-layer system integrating perception, inference, coordination, and reasoning across edge nodes**, with emphasis on reproducibility and system observability.

> Focus: validating architectural patterns and constraint-driven execution behavior under edge conditions (not a production deployment).

---

### Core System Layers

* **Interface Layer** → Signal ingestion (audio, vision, sensor data)
* **Knowledge Layer** → Structured representations and contextual mapping
* **Execution Pipeline (State-Ordered Processing)** →
  reproducible execution flow (state-machine style; stable given fixed inputs and weights)
* **Decision Layer** → Constraint-aware output generation
* **Coordination Layer (Gossip-Based Sync)** →
  lightweight state + metadata synchronization (Lamport ordering; no gradient sharing)

---

### System Characteristics

* Constraint-aware execution (latency, memory, compute limits)
* Edge-first design (cloud optional, not required for inference)
* Modular deployment across SBC-class hardware
* Reproducible pipelines (fixed seeds, controlled execution flow)

---

### Simplified System Flow

```text
Signals → Interface → Knowledge → Execution → Decision → Local Action
                              ↓
                       Experimentation Core
                              ↓
                    Coordination (Gossip Sync)
```

---

### Engineering Focus

* Trade-offs between **accuracy vs latency vs memory**
* Pipeline reproducibility vs probabilistic model behavior
* Edge-first deployment under CPU/SBC constraints
* Stability under noisy real-world inputs

---

### Example Execution Context (Validated)

* **Device (x86):** Intel i5-10210U, 8GB RAM
* **Device (ARM):** Raspberry Pi 4 (Cortex-A72, 4GB RAM)
* **Execution Mode:** CPU-only, single-thread (controlled variance)

#### Representative Results:

* **GNN inference latency (x86):**
  ~313–323 ms (10k-node graph, GraphSAGE, full-graph inference)

* **GNN inference latency (ARM):**
  ~1045–1280 ms (memory-bound; variance increases with graph density)

* **Quantization impact:**

  * Model size: 64 MB → 16 MB (~75% reduction)
  * Accuracy drop: ~0.9% (protein interaction classification task)
  * Latency: negligible change on x86, moderate improvement on ARM (~15–20%)

* **Distributed sync latency (mesh prototype):**
  ~200 ms mean
  jitter reduced from ±20 ms → ±5 ms after footprint optimization

---

### Observed Limitations / Edge Cases

* Quantization introduces **minor instability in edge cases** (dense subgraphs / high-degree nodes)
* Latency gains from INT8 are **limited on x86** (compute-bound stages dominate)
* Subprocess-based inference introduces ~10–15 ms overhead in current integration
* Gossip-based coordination may show **temporary state divergence under network partition**, resolving on reconnection

---

## Technical Stack

### Machine Learning & Edge Systems (Primary)

* PyTorch, TensorFlow Lite, PyTorch Geometric (GraphSAGE)
* NVIDIA Jetson, Raspberry Pi, SBC-class hardware
* INT8 quantization, memory-aware inference optimization

---

### Systems Architecture & Infrastructure

* Docker, Kubernetes, Linux systems
* Event-driven microservices, MQTT messaging
* REST / GraphQL APIs

---

### Backend Systems (Infrastructure Layer)

* PHP (Senior), Laravel
* PostgreSQL / MySQL, Redis

---

## Flagship Work

### Edge-GNN Systems Analysis

A systems-level investigation into **deploying Graph Neural Networks on edge hardware for biological interaction modeling**.

**Validated context:**

* Dataset: protein interaction graphs (~10k nodes / ~50k edges)
* Task: node classification (interaction likelihood proxy)
* Execution: CPU-only, fixed seed

Focus:

* GNN inference under hardware constraints
* Latency and memory trade-offs
* Biological interaction modeling
* Architecture patterns for edge ML systems

---

## System Evidence

To support architectural claims, systems demonstrate:

* Reproducible experiment pipelines (config-driven runs, fixed seeds)
* Measured latency + jitter across x86 and ARM
* Verified quantization trade-offs (size vs accuracy vs stability)
* Observable system behavior (logs, structured outputs)

---

## Selected Architecture Prototypes

### ZeroCloud-Edge-Mesh — Distributed Edge Coordination

A **local-first coordination prototype** for synchronizing edge nodes running GNN inference.

Validated behaviors:

* Lamport-clock-based causal ordering
* Gossip-based state synchronization
* Deterministic SQLite WAL persistence
* Recovery from node drop and network partition

---

### BioGraph-Edge-Quantizer — Resource-Aware GNN Optimization

A **quantization-aware GNN pipeline** for biological interaction modeling.

Validated:

* Dataset: ~10k node graph (STRING-derived)
* Accuracy: 91.8% → 90.9% (~0.9% drop)
* Model size reduction: ~75%
* ARM improvement: ~15–20% latency reduction (memory pressure effects)

---

### Med-Guard — Edge Clinical Monitoring

Prototype for **real-time physiological signal classification**.

* Input: audio / waveform signals
* Constraint: CPU-only inference
* Focus: latency stability under noisy input

---

### Eco-Guard Ramsar — Environmental Monitoring

Edge-based ecological monitoring system.

* Input: sensor + vision data
* Focus: low-frequency event detection under limited compute

---

## Design Philosophy

* Systems first, models second
* Constraints define architecture
* Reproducibility over implicit behavior
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
