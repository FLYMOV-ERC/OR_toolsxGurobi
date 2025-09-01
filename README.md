# VRPTW Solver Experiments: Gurobi vs OR-Tools

This repository contains two Jupyter notebooks that demonstrate how to model and solve a **Vehicle Routing Problem with Time Windows (VRPTW)** using two different solvers:

- [`ex_gurobi_b.ipynb`](ex_gurobi_b.ipynb) — implementation using the **Gurobi Optimizer**.
- [`ex_or_tools.ipynb`](ex_or_tools.ipynb) — implementation using **Google OR-Tools**.

The notebooks are intended for comparison of modeling styles, solver performance, and solution quality.

---

## Problem Description

The VRPTW problem involves scheduling a fleet of vehicles to serve a set of customers:
- Each customer has a demand and a time window \([a_i, b_i]\) when service must start.  
- Vehicles have limited capacity.  
- Travel times (or distances) are defined between locations.  
- The objective is to minimize the total distance traveled while satisfying all constraints.  

---

## Requirements

To run the notebooks, you need:

- Python 3.9+  
- Jupyter Notebook or JupyterLab  

### Python Packages

Install dependencies with:

```bash
pip install gurobipy ortools jupyter pandas numpy matplotlib
