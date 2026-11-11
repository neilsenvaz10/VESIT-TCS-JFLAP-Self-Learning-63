# Theory of Computer Science — JFLAP Self-Learning Assignment

**VESIT · Academic Year 2026–2027**

## Student Details

| Field | Detail |
|---|---|
| **Name** | Neilsen Vaz |
| **Roll Number** | 63 |
| **Class** | TE Computer Engineering, Sem V, D12A |
| **Academic Year** | 2026-2027 |
| **Subject** | Theory of Computer Science |
| **Subject Code** | 26CMPC51 |

## Assignment Title

**JFLAP Self-Learning Experiments in Automata, Grammars, and Computation**

## Experiments (First 5)

| # | Experiment | Description | Folder | Files | Status |
|--:|---|---|---|---|---|
| 1 | **DFA** | DFA recognizing binary strings ending in `01`. Three states tracking the longest suffix matching `01`. | [01-DFA](experiments/01-deterministic-finite-automata-dfa/) | [`63_Neilsen_Vaz_DFA_10-11-2026.jff`](experiments/01-deterministic-finite-automata-dfa/63_Neilsen_Vaz_DFA_10-11-2026.jff) | ✅ Complete |
| 2 | **NFA** | NFA recognizing strings over {a,b} containing the substring `ab`. The NFA nondeterministically guesses where `ab` begins. | [02-NFA](experiments/02-nondeterministic-finite-automata-nfa/) | [`63_Neilsen_Vaz_NFA_10-11-2026.jff`](experiments/02-nondeterministic-finite-automata-nfa/63_Neilsen_Vaz_NFA_10-11-2026.jff) | ✅ Complete |
| 3 | **NFA-to-DFA Conversion** | Subset construction converting an NFA for strings ending in `01` to an equivalent DFA. | [03-NFA-to-DFA](experiments/03-nfa-to-dfa-conversion/) | [`63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff`](experiments/03-nfa-to-dfa-conversion/63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff) | ⚠️ Pending verification — converted DFA file present but GUI conversion not yet verified in JFLAP |
| | | | | [`63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff`](experiments/03-nfa-to-dfa-conversion/63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff) | |
| 4 | **DFA Minimization** | Four-state DFA minimized to an equivalent three-state DFA for binary strings ending in `01`. Includes manually saved minimized result. | [04-DFA-Minimization](experiments/04-dfa-minimization/) | [`63_Neilsen_Vaz_DFA_Minimization_Original_DFA_10-11-2026.jff`](experiments/04-dfa-minimization/63_Neilsen_Vaz_DFA_Minimization_Original_DFA_10-11-2026.jff) | ✅ Complete |
| | | | | [`63_Neilsen_Vaz_DFA_Minimization_Minimized_DFA_10-11-2026.jff`](experiments/04-dfa-minimization/63_Neilsen_Vaz_DFA_Minimization_Minimized_DFA_10-11-2026.jff) | |
| | | | | [`63_Neilsen_Vaz_DFA_Minimized_11-11-2026.jff`](experiments/04-dfa-minimization/63_Neilsen_Vaz_DFA_Minimized_11-11-2026.jff) *(manually saved)* | |
| 5 | **DFA to Regular Grammar** | DFA for strings over {a,b} ending in `ab` converted to an equivalent right-linear grammar. Includes manually exported grammar file. | [05-DFA-to-Regular-Grammar](experiments/05-dfa-to-regular-grammar-conversion/) | [`63_Neilsen_Vaz_DFA_to_Regular_Grammar_Original_DFA_10-11-2026.jff`](experiments/05-dfa-to-regular-grammar-conversion/63_Neilsen_Vaz_DFA_to_Regular_Grammar_Original_DFA_10-11-2026.jff) | ✅ Complete |
| | | | | [`63_Neilsen_Vaz_DFA_to_Regular_Grammar_Converted_Grammar_10-11-2026.jff`](experiments/05-dfa-to-regular-grammar-conversion/63_Neilsen_Vaz_DFA_to_Regular_Grammar_Converted_Grammar_10-11-2026.jff) | |
| | | | | [`63_Neilsen_Vaz_DFA_to_Regular_Grammar_11-11-2026.jff`](experiments/05-dfa-to-regular-grammar-conversion/63_Neilsen_Vaz_DFA_to_Regular_Grammar_11-11-2026.jff) *(manually saved)* | |

## How to Open and Run in JFLAP

1. Install or use **JFLAP 7.1** (or a version compatible with `.jff` files).
2. Open a numbered experiment folder and use **File → Open** to load its `.jff` file.
3. Follow that folder's `README.md` for the relevant run/parse menu and expected test cases.
4. For conversion experiments (3, 4, 5), run identical strings against both original and converted models to verify equivalence.

## File Naming Convention

```
63_Neilsen_Vaz_Topic_DOP.jff
```

- **63** — Roll number
- **Neilsen_Vaz** — Student name
- **Topic** — Experiment topic (e.g., `DFA`, `NFA`, `NFA_to_DFA_Converted_DFA`)
- **DOP** — Date of Performance (DD-MM-YYYY format)

## Verification Notes

- XML parsing and JFF structure checks passed for all files (see `tools/validate_12_experiments.py`).
- Offline language/equivalence checks passed for DFA, NFA, and conversion pairs.
- **No GUI screenshots are included** — the JFLAP GUI was unresponsive to automation during preparation. Each experiment README contains manual steps for completing GUI verification.
- Experiment 3 (NFA-to-DFA) has the converted DFA file but the JFLAP subset construction process has not been independently verified in the GUI.

## Repository Structure

```
├── experiments/
│   ├── 01-deterministic-finite-automata-dfa/
│   ├── 02-nondeterministic-finite-automata-nfa/
│   ├── 03-nfa-to-dfa-conversion/
│   ├── 04-dfa-minimization/
│   └── 05-dfa-to-regular-grammar-conversion/
├── .gitignore
└── README.md
```

> **Note:** Experiments 6–12, the 35 module folders, and supporting tools remain in the local project and are preserved. Only the first 5 experiments are published in this submission.
