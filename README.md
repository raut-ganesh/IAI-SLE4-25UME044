# SLE-4: Final Viva & Architecture Decision Record (ADR)

## Course Information

* **Course:** 02AML204 – Introduction to Artificial Intelligence
* **Name:** Ganesh Ujesh Raut
* **PRN:** 25UME044
* **Division:** A
* **Institute:** DKTE Society's Textile and Engineering Institute, Ichalkaranji

## Overview

This repository contains my SLE-4 submission for the Introduction to Artificial Intelligence course. It summarizes my learning from SLE-1, SLE-2, and SLE-3 and presents an Architecture Decision Record (ADR) based on my graph-search profiling experiments.

## Architecture Decision Record (ADR)

**Decision:** Select Breadth-First Search (BFS) for the tested graph-search scenario based on the recorded profiling results.

### Context

In SLE-2, I compared Breadth-First Search (BFS) and Depth-First Search (DFS) using a binary-tree graph containing 65,535 vertices and 65,534 edges. I used Python, VS Code Terminal, and Py-Spy to examine their performance over three runs.

### Profiling Results

| Metric                 |     BFS |      DFS |
| ---------------------- | ------: | -------: |
| Average execution time | 4.53 ms | 22.33 ms |
| Nodes expanded         |  15,000 |   54,472 |

Based on these recorded results, BFS performed better in my tested scenario. This decision does not mean BFS is always faster than DFS.

### Alternatives Considered

* **BFS:** Explores nodes level by level using a queue.
* **DFS:** Explores deeper paths first using a stack or recursion.

### Consequences

**Positive:**

* Lower average execution time in the recorded experiment.
* Fewer expanded nodes in the recorded results.
* Can find the shortest path in an unweighted graph.

**Trade-offs:**

* BFS may require more memory to store nodes in a queue.
* Performance can vary with graph structure and search requirements.
* Further experiments are needed before generalizing this decision.

## SLE Journey

### SLE-1: AI-Based Smart Home Agent

Developed a simple Python-based rule-driven agent using temperature, light, and motion conditions.

### SLE-2: BFS vs DFS Profiling

Compared BFS and DFS on a binary-tree graph and recorded execution time and expanded-node results.

### SLE-3: Graph Search & Profiling Engine

Designed the system architecture using the C4 model: Context, Container, Component, and Code.

### SLE-4: Final Viva & ADR

Documented the architecture decision, justified it using profiling results, summarized my learning, and prepared viva questions.

## AI Contribution

ChatGPT was used to help understand BFS and DFS, explain code, organize the C4 architecture, and interpret profiling results. I ran the programs, checked their outputs, compared the performance results, and studied the architecture diagrams and main functions.

## References

* [SLE-1: AI-Based Smart Home Agent](https://github.com/raut-ganesh/IAI-SLE1-25UME044)
* [SLE-2: BFS vs DFS Profiling](https://github.com/raut-ganesh/IAI-SLE2-25UME044)
* [SLE-3: Graph Search & Profiling Engine](https://github.com/raut-ganesh/IAI-SLE3-25UME044)

## Conclusion

This work helped me understand AI agents, graph-search algorithms, performance profiling, and software architecture. The recorded experiments supported selecting BFS for the specific graph-search scenario tested.
