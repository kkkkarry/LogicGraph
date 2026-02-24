# LogicGraph: Benchmarking Multi-Path Logical Reasoning via Neuro-Symbolic Generation and Verification
### 📖 Overview

Evaluations of large language models (LLMs) primarily emphasize convergent logical reasoning, where success is defined by producing a single correct proof. [cite_start]However, many real-world reasoning problems admit multiple valid derivations, requiring models to explore diverse logical paths rather than committing to one route. 

To address this limitation, we introduce **LogicGraph**, the first benchmark aimed to systematically evaluate multi-path logical reasoning. [cite_start]LogicGraph is constructed via a neuro-symbolic framework that leverages backward logic generation and semantic instantiation. 

### ✨ Key Features

* **Multi-Path & High-Depth:** Each query in LogicGraph admits 2 to 19 valid proof paths. [cite_start]The benchmark features an average reasoning depth of 6.01 steps.
* **Exhaustive Ground Truth:** Each instance is associated with an exhaustive set of minimal proofs.
* **Inherent Logical Distractions:** The dataset introduces structural distractions where a premise can be crucial for one valid path yet distracting for another. 
* **Neuro-Symbolic Evaluation:** We propose a reference-free neuro-symbolic evaluator that translates generated natural language steps into formal logic and verifies them using a symbolic solver (Prover9).

### 📊 Dataset

The LogicGraph dataset is fully open-source and available in this repository. It consists of 900 instances divided into three difficulty tiers based on the number of valid derivation paths: Small, Medium, and Large.

### 💻 Code Status
Currently, the dataset is fully public. The neuro-symbolic generation pipeline, Prover9 evaluation scripts, and model inference code are being finalized and will be released soon.
