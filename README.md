# Swapin Vidya

**Systems Architect | Edge AI | ML Systems Design**

**Primary focus: Edge-constrained ML systems (GNN workloads, structured pipelines, and distributed edge coordination).**

I design and build **edge-native AI systems** where real-world constraints—latency, memory, and reliability—directly shape system architecture.

With a strong foundation in backend engineering and distributed systems, my work focuses on:

* **Edge AI pipelines (audio, vision, biological signals)**
* **Graph-based ML systems under resource constraints (Edge-GNN)**
* **Distributed coordination across edge nodes (gossip / federated patterns)**
* **Reproducible ML experimentation and benchmarking systems**

---

```text
All systems and prototypes presented below are modular research and engineering foundations that inform the PeachbotAI architecture.
```

---

# Flagship System — PeachbotAI

**PeachbotAI is a hybrid edge AI system for safety-critical environments, combining deterministic orchestration with controlled machine learning components.**

It is designed for **real-time, on-device intelligence** in domains such as healthcare, environmental monitoring, and biological systems—where **auditability, latency, and reliability are critical**.

**Status:** Validated MVP → Early deployment transition

* Multi-layer architecture integrated and tested
* Functional edge AI modules operational
* Ongoing optimization for real-world deployment

---

## Architectural Principle

Peachbot follows a **system-centric architecture**:

* Deterministic orchestration governs system behavior
* ML models (GNNs, LLMs) are **supporting components**, not decision-makers
* Outputs are validated through **safety and policy layers**

This ensures **controlled, auditable system behavior under real-world constraints**.

---

## Core Architecture Layers

* **Input Layer** → real-world signals (clinical, environmental, biological)
* **Preprocessing Layer** → normalization and structuring
* **Semantic Extraction Layer** → ML/NLP-based structured interpretation
* **Knowledge Layer (Versioned KG)** → domain grounding (clinical, ecological, biological)
* **Edge Intelligence Layer (SBC)** → state-centric execution and reasoning
* **Safety Layer** → constraint enforcement and validation
* **Output Layer** → alerts, recommendations, structured outputs
* **Cloud Coordination Layer (FILA)** → metadata-only synchronization and validation

---

## SBC (State-Based Computation)

Implemented as:

* state-machine–style execution pipeline
* structured state → interpretation → constrained output
* reproducible execution given fixed inputs and weights

👉 Ensures **traceability and system-level control**, not deterministic ML predictions.

---

## FILA (Federated Intelligence Layer)

* Coordination layer for distributed edge nodes

* Handles:

  * metadata synchronization
  * state consistency
  * validation signals

* Uses:

  * gossip-style communication
  * partial system visibility

👉 Does **not perform model training or gradient sharing**.

---

## System Behavior

* Learning is localized and continuous
* Intelligence emerges across nodes
* Cloud provides coordination—not centralized control

---

## Validated System Evidence

### Hardware Context

* Intel i5-10210U (8GB RAM)
* Raspberry Pi 4 (4GB RAM)
* CPU-only execution

---

### Edge-GNN (BioGraph-Edge-Quantizer)

* Dataset: ~10k node protein interaction graph (~50k edges)
* Task: node classification

**Results:**

* Accuracy: 91.8% → 90.9% (~0.9% drop)
* Model size: 64MB → 16MB (~75% reduction)
* ARM latency improvement: ~15–20%
* Observation: performance remains **memory-bound**, not compute-bound

---

### Coordination Behavior (ZeroCloud-Edge-Mesh)

* Mean sync latency: ~204 ms
* Jitter reduced: ±20 ms → ±5 ms after optimization

**Failure handling:**

* Network partition → eventual convergence
* Node drop → recovered via next sync cycle
* Duplicate messages → deterministic resolution (LWW strategy)

---

## Observed Limitations

* Quantization introduces **minor instability in dense graph regions**
* Limited latency improvement on x86 (compute bottlenecks dominate)
* Gossip coordination may cause **temporary state divergence**
* Subprocess-based execution adds ~10–15 ms overhead

---

## Deployment Signal

* Environmental system validated at **Sasthamkotta Ramsar Site (India)**
* Edge-based ecological monitoring tested under real-world constraints
* System transitioning toward deployment-scale infrastructure

---

## Role of AI Models

* Used for:

  * perception
  * pattern recognition
  * contextual reasoning

* Always:

  * constrained by system logic
  * validated before influencing outputs

👉 Peachbot is **system-driven, not model-driven**.

---

# ⚙️ Technical Stack

### Machine Learning & Edge Systems

* PyTorch, TensorFlow Lite, PyTorch Geometric (GraphSAGE)
* SBC-class hardware (Jetson, Raspberry Pi)
* INT8 quantization, memory-aware optimization

---

### Distributed Systems

* Gossip protocols, Lamport clocks
* SQLite WAL persistence
* Event-driven coordination

---

### Backend & Infrastructure

* PHP (Laravel), PostgreSQL, Redis
* Docker, Kubernetes
* REST / GraphQL APIs

---

# Selected System Prototypes (Foundational Work)

These are **independent prototypes and research systems** that informed the PeachbotAI architecture.

They represent **focused explorations of constraints, subsystems, and design patterns**, later refined into a unified system.

---

### BioGraph-Edge-Quantizer

Resource-aware GNN inference system:

* INT8 quantization (~75% reduction)
* Accuracy trade-offs (~0.9% drop)
* Memory-bound inference behavior

---

### ZeroCloud-Edge-Mesh

Distributed coordination prototype:

* Gossip-based synchronization
* Lamport clock ordering
* SQLite WAL persistence
* Eventual consistency under failure

---

### Med-Guard

Physiological signal monitoring prototype:

* Real-time signal processing
* CPU-only inference
* Stability under noisy inputs

---

### Eco-Guard Ramsar

Environmental monitoring system:

* Field deployment (Ramsar Site, India)
* Edge-based sensing and detection
* Low-frequency event monitoring

---

### Relationship to PeachbotAI

These systems contributed architectural insights:

* GNN optimization → Edge Intelligence Layer
* Distributed coordination → FILA design
* Domain systems → Input and application validation

👉 PeachbotAI is a **refined architecture built from these validated experiments**, not a direct aggregation.

---

# Design Philosophy

* Systems first, models second
* Constraints define architecture
* Reproducibility over abstraction
* Measurable trade-offs over theoretical performance
* Hybrid control (deterministic orchestration + ML support)

---

# Background

* MBBS Coursework — Government Medical College
* Diploma in Business Administration (In Progress)

---

# Availability

Open to:

* Systems architecture roles
* Edge AI / ML systems engineering
* Distributed systems / platform engineering
* Applied research collaborations

---

