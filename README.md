# LowRankDynamics

## Overview
`LowRankDynamics` is a repository containing example Jupyter notebooks that demonstrate the use of the LR-TDVP method  introduced in - Gravina, Luca, and Vincenzo Savona. [Adaptive variational low-rank dynamics for open quantum systems](https://arxiv.org/abs/2312.13676).
This method improves the efficiency with which low-entropy dissipative many-body systems can be simulated. The method relies on the assumption that in such systems the dynamics can be accurately captured by including a limited number of states in the ansatz for the statistical mixture. Leveraging the time-dependent variational principle, the method identifies the optimal subset of states over which to decompose the Lindblad master equation, dynamically modifying this low-rank basis to adapt to changes in the system's entropy. This methodology offers substantial computational advantages over existing adaptive low-rank schemes in terms of both computational time and memory requirements.

The code for the LowRank dynamics method itself is implemented in the Julia [`QuantumToolbox.jl`](https://github.com/albertomercurio/QuantumToolbox.jl) library. This repository, while it does not contain the source code of the method, it provides illustrative examples and guides on how to reproduce many of the plots and results presented in the paper.

## Getting Started
To use the examples provided in this repository, you will need to have Julia installed on your system, along with the `QuantumToolbox.jl` package. The examples are provided in the form of Jupyter notebooks, which allow for an interactive exploration of the LowRank dynamics method.

### Prerequisites
- Julia (version requirement as per `QuantumToolbox.jl`)
- Jupyter Notebook or JupyterLab
- QuantumToolbox.jl Julia package

### Installation
1. **Install Julia:** Follow the instructions on the [official Julia website](https://julialang.org/downloads/) to download and install Julia for your operating system.

2. **Set up Jupyter Notebook:** If you haven't already, install Jupyter Notebook or JupyterLab. This can be done through Python's pip package manager:
   ```bash
   pip install notebook
   ```
   or 
   ```bash
   pip install jupyterlab
   ```
3. **Install QuantumToolbox.jl:** Open the Julia and add the `QuantumToolbox.jl` package by entering the Julia REPL and typing:
   ```bash
    using Pkg
    Pkg.add("QuantumToolbox")
   ```

### Examples
The repository contains notebooks showcasing different use cases of the LR-TDVP method in both spin and bosonic systems. By extending the examples shown in the notebooks, you can reproduce many of the plots presented in the paper.
