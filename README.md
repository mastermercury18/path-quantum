# 🧬 Quantum-Guided Apoptosis Pathway Selector

**Harnessing Quantum Optimization with Perceval to Model and Evaluate Protein Cascades for Cancer Suppression**

---

## 🧠 Overview

This project leverages a **quantum-inspired approach to systems biology**, using photonic quantum computing via the **Perceval** framework to determine optimal protein signaling cascades that lead to **apoptosis** — the natural process of programmed cell death. By simulating synthetic biological networks as weighted graphs and mapping them to **QUBO (Quadratic Unconstrained Binary Optimization)** problems, this system efficiently identifies paths most likely to suppress cancer.

The backend is built in Python and integrates multiple HTML-based UI options for user input. At its core, the quantum pipeline selects shortest apoptotic pathways by analyzing probabilistic outputs from a photonic interferometer that encodes biological constraints.

---

## 🔍 How It Works

### 1. **Graph Generation from Protein Cascades**
- The user selects a **synthetic signaling network** which is represented as a **directed graph**.
- Each **protein interaction** is converted into an edge with a specific weight, derived from simulated activation probabilities or experimental heuristics.

### 2. **QUBO Mapping**
- The graph is transformed into an **adjacency matrix**, encoding:
  - Edge weights (biological cost/efficiency)
  - Node constraints (e.g., inhibition, dual activation)
- This matrix is used to formulate a **QUBO problem**, aiming to minimize the total signaling cost while reaching apoptotic targets.

### 3. **Quantum Circuit Construction**
- Using the **Perceval** quantum photonic framework, the adjacency matrix is embedded into a **linear interferometer**.
- A series of **beam splitters and phase shifters** are configured to simulate quantum walk dynamics over the protein network.

### 4. **Quantum Path Sampling**
- The interferometer samples **Fock states**, simulating boson interference patterns.
- High-probability output modes correspond to **constructively interfering cascades** — i.e., biologically plausible and efficient signaling paths.

### 5. **Result Analysis**
- Quantum sampling results are mapped back to the biological graph.
- Optimal paths leading to apoptosis are extracted and visualized.
- Output probabilities are used to infer **confidence scores** for each path.

---

## ⚗️ Key Technologies

- **🧠 Perceval** – Photonic quantum simulator for QUBO encoding.
- **📊 NetworkX** – Graph generation and manipulation.
- **📈 Numpy + Pandas** – Data preparation from synthetic CSVs.
- **🌐 HTML UI** – Input collection for biological conditions and pathway simulation.
- **📄 Flask** – (Optional) Can be integrated to serve the tool as a web interface.

---

## 🧪 Example Use Case

1. User selects a specific cell signaling pathway
2. The system builds a graph with apoptotic goals (e.g., p53 activation).
3. Using quantum walk-based simulation, it identifies the best cascade through proteins like AKT, PUMA, BAX, or Caspases.
4. Displays:
   - Shortest path
   - Probabilistic confidence
   - Biological interpretation of selected path

---

## 🧬 Why Quantum?

- **Entanglement-like correlations** help model combinatorial dependencies in protein activation.
- Quantum walks capture **constructive/destructive interference**, which models how simultaneous pathways may enhance or inhibit apoptosis.
- Faster convergence compared to brute-force combinatorial searches in classical simulation — particularly beneficial for **large protein interaction networks**.
