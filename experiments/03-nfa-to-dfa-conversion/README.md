# Experiment 03: NFA to DFA Conversion

**Student:** Neilsen Vaz Â· **Roll No.:** 63 Â· **Class/Division:** T.E. Computer Engineering / D12A Â· **Semester:** V Â· **AY:** 2026â€“2027 Â· **Subject Code:** 26CMPC51

## Objective and model

Convert the NFA for binary strings ending in `01` by subset construction. The subset DFA accepts exactly the same language.

## Files

- [63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff](63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff)
- [63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff](63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff)

## JFLAP procedure

1. Open JFLAP 7.1.
2. Open the listed machine file(s) with **File â†’ Open**.
3. Use **Input â†’ Multiple Run** for automata and transducers; use the relevant grammar parse or TM run option for those machine types.
4. Compare outputs with the table below. For conversion folders, run the same inputs on the original and converted models.

## Test inputs and expected behavior

| Input | Expected behavior |
|---|---|
| `01` | Accept in both |
| `101` | Accept in both |
| `1101` | Accept in both |
| `Îµ` | Reject in both |
| `10` | Reject in both |
| `011` | Reject in both |

## Verification status

> **âš ï¸ Pending verification:** The converted DFA file was generated programmatically using subset construction logic. Automated XML parsing and structural validation passed, and offline equivalence checks confirmed both models accept the same strings for bounded-length inputs. However, the actual JFLAP GUI conversion process (Convert â†’ Convert to DFA) has **not** been independently verified. The converted DFA file should be validated manually in JFLAP by running the original NFA through the subset construction tool and comparing the result.

Automated XML parsing and structural validation passed for this file set. Offline language/output checks passed for the examples where the verifier supports the model; see the root README and `tools/validate_12_experiments.py`. Exact DFA equivalence checks passed for the NFA-to-DFA and minimization pairs. Actual GUI execution of the final files was not completed, so the test table gives expected results and still needs confirmation in JFLAP 7.1.

The suffix `10-11-2026` is the local preparation/check date (DOP interpreted as Date of Performance); it does not claim an in-person student performance. Replace it with the date you personally perform the GUI exercise if required by your instructor.

## GUI Verification

> **⚠️ Partial verification:** The original NFA (Ending_01_NFA.jff) was opened in JFLAP and tested with Multiple Run. The converted DFA file has not been independently verified via JFLAP's Convert → Convert to DFA tool.

- `63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff` — ✅ Original NFA GUI-tested; accepts/rejects strings ending in `01` correctly.
- `63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff` — ⚠️ Pending verification of JFLAP subset construction.

### Screenshot

![NFA-to-DFA Original NFA Multiple Run](63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.png)