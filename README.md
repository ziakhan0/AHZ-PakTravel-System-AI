# PakTravel AI System
### AL2002 — Artificial Intelligence | Spring_2026
**FAST NUCES — Chiniot-Faisalabad Campus**

---

## Overview

PakTravel AI System is a semester project that builds an intelligent road travel assistant for a fictional Pakistani bus company. The project covers five core AI techniques — search algorithms, propositional logic, constraint satisfaction, neural networks, and unsupervised learning — all connected through the story of a student travelling from Karachi to Multan.

---

## Project Structure

```
PakTravel_AI_System/
├── PakTravel_AI_System.ipynb   # Main notebook (all 5 parts)
├── aima3/                      # AIMA Python library (offline)
├── requirements.txt            # Python dependencies
└── README.md                   # Documentation
```

---

## Modules

| Part | Topic | Technique |
|------|-------|-----------|
| 1 | Route Planning | UCS, A\*, Bidirectional Search, Relay Planner |
| 2 | AI Legal Advisor | Propositional Logic, Forward Chaining (AIMA3) |
| 3 | Bus Scheduling | CSP, Backtracking, MRV, AC3 |
| 4 | Delay Prediction | Artificial Neural Network (sklearn + NumPy) |
| 5 | Traveller Clustering | K-Means, Elbow Method |

---

## Getting Started

### Option 1 — Install dependencies first (recommended)

```bash
pip install -r requirements.txt
```

Then open and run the notebook:

```bash
jupyter notebook PakTravel_AI_System.ipynb
```

### Option 2 — Auto setup inside notebook

Run the first setup cell in the notebook. It installs all required packages automatically, then run all remaining cells.

---

## AIMA3 Usage (Part 2)

Part 2 uses the `aima3` library for propositional logic. Basic usage:

```python
from aima3.logic import PropDefiniteKB, expr, pl_fc_entails

kb = PropDefiniteKB()
kb.tell(expr('Speed_Above_Limit ==> Challan_Issued'))
kb.tell(expr('Speed_Above_Limit'))

print(pl_fc_entails(kb, expr('Challan_Issued')))  # True
```

---

## Requirements

- Python 3.8+
- numpy
- pandas
- matplotlib
- scikit-learn
- networkx
- aima3

---

## Notes

- All five parts are in a single `.ipynb` file as required by the project instructions.
- Each part begins with a markdown cell describing the scenario and methodology.
- Part 2 uses `PropDefiniteKB` from `aima3`. If the library is unavailable, a custom implementation is included as fallback.
- Visualizations (road network graph, confusion matrix, elbow curve, scatter plot) are generated inline inside the notebook.

---

*AL2002 Artificial Intelligence | Spring 2026 | FAST NUCES Chiniot-Faisalabad*
