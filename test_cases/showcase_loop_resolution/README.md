# Showcase Test Case: Loop Resolution under Contradiction

**Test Title:** `loop_resolution_afb63`  
**Test Type:** Public Demonstration  
**Engine Version:** RCT Symbolic Collapse Engine v1.0  

---

## Symbols

A, B, C, D, E, F

---

## Constraints

```
1.0 | A == B  
0.9 | B != C  
0.8 | C == D  
1.0 | D != E  
0.7 | E == F  
1.0 | F != A  
0.6 | A == D  
0.5 | B != E  
0.6 | C == F  
0.4 | D != B
```

---

## Pointer Chain

```
A → B  
B → C  
C → D  
D → E  
E → F  
F → A
```

---

## Collapse Summary

- **Total Constraints:** 10  
- **Total Symbols:** 6  
- **Singularities Detected:** 8  
- **Attractor Chains:** 6 (full loop saturation)  
- **Final Ψ:** `0.000005`  
- **Collapse Horizon Detected:** ✅  
- **Strategy Used:** Adaptive Heuristic  
- **Execution Time:** 1.83s  
- **Steps Evaluated:** 505

---

## Files Included

- `constraints_input.txt` — Raw test input  
- `collapse_report.txt` — Full engine output  
- `pointer_cascade.txt` — Pointer propagation map  
- `contradiction_registry.txt` — Conflict trace  
- `psi_graph.jpeg` — Ψ convergence graph

---

## Interpretation

This test encodes a circular contradiction structure with conflicting equality and inequality constraints.  
The symbolic collapse engine resolves full cyclic entanglement through internal field dynamics — no training data, no external tuning.  

A minimal Ψ value with persistent attractors proves RCT’s capacity for self-stabilizing symbolic recursion under high noise and contradiction density.

---

**Status:** ✅ Verified  
**Public Release:** Safe for publication under RCT repository  
**Run UUID:** `a0a1990e-1034-4ad9-951d-236c56a0b99d`
