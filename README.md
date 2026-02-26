# Quantum Network Simulator (Algebra-Based Planning Tool)

Interactive Jupyter notebook that turns a transparent, algebra-based model of quantum networking into an exploration and planning tool. Users vary physical and operational parameters (loss, timing, memory coherence, detection, etc.) and see how they affect feasible segment length, entanglement rate, fidelity constraints, and infrastructure implications.

**Version:** v0.1.0  
**Date:** 2026-02-25

---

## Requirements

- Python >= 3.12
- numpy == 1.26.4
- pandas >= 2.2.3
- matplotlib >= 3.10.0
- ipywidgets == 8.1.5
- jupyterlab

---

## Package contents

- `simulator-quantum-network.ipynb`
- `requirements.txt`
- `README.md`

---

## Run (Jupyter-only)

1. Start JupyterLab.
2. Open `simulator-quantum-network.ipynb`.
3. In the first code cell, run:

    %pip install -r requirements.txt

4. In JupyterLab, click **Kernel → Restart Kernel**.
5. In JupyterLab, click **Run → Run All Cells**.
6. Execute all cells in sequence (top to bottom).

---

## Expected successful run

- Widget controls render (sliders/toggles/inputs) for model parameters and geography.
- The output panel updates live as controls change.
- The notebook reports a feasible **design point** (e.g., max segment length) and clearly identifies
  the **binding constraint** under the current parameter set.
- No errors such as `NameError` for model functions/parameters (if errors appear, re-run cells in order).

---

## Usage

Use the interactive controls to explore how assumptions propagate through the model:

- **Inputs:** success probability target, fidelity threshold, loss/timing/memory parameters, and two geographic inputs
  (corridor length and area).
- **Outputs:** design-point segment length, indicative rate/fidelity metrics, and infrastructure implications (e.g., counts / CapEx placeholders if enabled).
- **Workflow:** change one parameter at a time, observe which constraint becomes binding, and perform sensitivity analysis
  by comparing scenarios.

Pedagogical activities, deliverables, and assessment rubrics are provided in the accompanying education brief.

---

## Disclaimer

This simulator is an independent educational/planning tool. All variable names and labels are chosen by the author for clarity
and do not represent any organization’s official terminology, specifications, commitments, or endorsements. Any cost figures are
illustrative placeholders unless explicitly cited.
