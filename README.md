

---

## Solver Notes
- The primary approach uses **MILP with PuLP/OR-Tools** (binary facility-open variables).
- This repository also includes a **fallback solver** (used here) with `scipy.optimize.linprog` for transport + a **greedy facility-closing heuristic** to account for fixed costs.
- To switch to MILP, install `pulp` (CBC) or `ortools` and adapt the solver in `src/optimize_network.py`.

