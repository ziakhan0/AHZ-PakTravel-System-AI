PakTravel AI System — AL2002 Spring 2026
FAST NUCES Chiniot-Faisalabad Campus
=========================================

FILES IN THIS ZIP
-----------------
  PakTravel_AI_System.ipynb   Main notebook (all 5 parts)
  aima3/                      AIMA Python library (pre-included)
  requirements.txt            All package requirements
  README.txt                  This file

HOW TO RUN — 2 OPTIONS
-----------------------

OPTION 1 (Recommended — Internet not needed for aima3):
  1. Extract this zip folder
  2. Open terminal in the extracted folder
  3. Run: pip install -r requirements.txt
  4. Open: PakTravel_AI_System.ipynb in Jupyter
  5. Run all cells

OPTION 2 (Auto-install from notebook):
  1. Extract this zip
  2. Open PakTravel_AI_System.ipynb
  3. Run the FIRST CELL ("SETUP CELL") — it installs everything
  4. Run all remaining cells

AIMA3 LIBRARY (Part 2)
-----------------------
  The aima3/ folder is included so you do NOT need internet
  to get the AIMA library. If Python does not pick it up
  automatically, run this from the project folder:
    pip install aima3

  Part 2 uses:
    from aima3.logic import PropDefiniteKB, expr, pl_fc_entails
    kb = PropDefiniteKB()
    kb.tell(expr('Speed_Above_Limit ==> Challan_Issued'))
    pl_fc_entails(kb, expr('Challan_Issued'))

PARTS SUMMARY
-------------
  Part 1 — Route Planning      : UCS, A*, Relay, Bidirectional
  Part 2 — AI Legal Advisor    : aima3 PropDefiniteKB, 15 rules
  Part 3 — Bus Scheduling      : CSP, Backtracking, MRV, AC3
  Part 4 — Delay Prediction    : sklearn ANN + NumPy ANN
  Part 5 — Traveller Clustering: K-Means, Elbow Method
