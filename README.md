# Graph-Theory-Book-Report
This repository contains a book report on Hamiltonian Graphs, focusing on fundamental theorems, conditions for Hamiltonian cycles, and computational verification. It explores Hamiltonian paths and includes proofs of key theorems, along with Python code for practical verification and LaTeX documents.

# Hamiltonian Graphs: Theorems, Proofs, and Computational Verification

## Overview

This repository provides an in-depth report and analysis of **Hamiltonian Graphs**, an essential concept in graph theory that deals with the existence of cycles visiting all vertices of a graph exactly once. The report combines theoretical exploration with practical computational verification, focusing on both classic theorems and modern applications.

Hamiltonian graphs have significant relevance in various fields such as optimization, network design, and algorithmic problem solving. The report aims to cover both the fundamental and advanced aspects of Hamiltonian graph theory, supported by mathematical proofs and Python implementations.

## Key Concepts Covered:

### 1. **Hamiltonian Path and Hamiltonian Cycle**:
- **Hamiltonian Path**: A path that visits every vertex in a graph exactly once.
- **Hamiltonian Cycle**: A cycle that visits every vertex in the graph exactly once and returns to the starting vertex.
- **Hamiltonian Graph**: A graph that contains a Hamiltonian cycle.

### 2. **Key Theorems and Proofs**:
The report explores some of the most important theorems in Hamiltonian graph theory, including:
- **Dirac's Theorem**: If every vertex of an \(n\)-vertex graph has degree at least \(n/2\), then the graph is Hamiltonian.
- **Ore's Theorem**: If the sum of degrees of any two non-adjacent vertices in an \(n\)-vertex graph is at least \(n\), then the graph is Hamiltonian.
- **Bondy-Chvátal Theorem**: A graph is Hamiltonian if its closure is Hamiltonian.
- **Pósa's Theorem**: Provides sufficient conditions for a graph to have a Hamiltonian cycle based on vertex degrees.

Each of these theorems is not only proved but also demonstrated through computational examples in Python.

### 3. **Computational Verification**:
The repository includes Python scripts that implement algorithms to check whether specific graphs, such as the Peterson graph and random planar graphs, contain Hamiltonian cycles. The report discusses the use of the `NetworkX` library in Python for generating graphs and running algorithms to validate Hamiltonian cycles.

Example implementations include:
- Checking for Hamiltonian cycles in random planar graphs.
- Using exhaustive search algorithms to verify the presence or absence of Hamiltonian cycles in specific graphs like the Peterson graph.

### 4. **Applications**:
Hamiltonian graph theory has wide applications in:
- **Optimization**: Problems like the **Traveling Salesman Problem** (TSP), which seeks the shortest Hamiltonian cycle in a weighted graph.
- **Network Design**: Ensuring efficient communication routes by finding Hamiltonian paths or cycles.
- **Algorithmic Challenges**: Many computational problems in operations research rely on Hamiltonian cycles.

## Structure of the Repository:
- **Main Report**: The LaTeX code and compiled PDF of the book report on Hamiltonian graphs are available in the `report/` folder.
- **Python Code**: The `code/` folder contains Python scripts that implement graph algorithms for Hamiltonian cycle detection, such as the Peterson graph analysis and random planar graph generation.
  - **petersen_graph.py**: A script that uses brute-force search to check for Hamiltonian cycles in the Peterson graph.
  - **random_planar_graph.py**: A script that generates random planar graphs and checks them for Hamiltonian cycles.
  
## How to Use This Repository:
1. **Compiling the LaTeX Report**: The LaTeX file can be found in the `report/` folder. You can compile it using any LaTeX editor to generate the final PDF report.
2. **Running Python Scripts**: Navigate to the `code/` folder and run the provided Python scripts to see the computational results.
   - Example: Run `petersen_graph.py` to check for Hamiltonian cycles in the Peterson graph:
     ```bash
     python petersen_graph.py
     ```

## Requirements:
- **Python 3.x**
- **NetworkX** library for graph generation and manipulation.
- **Matplotlib** for graph visualization.
  
  You can install the required libraries using the following:
  ```bash
  pip install networkx matplotlib
