# Experiment 02: Nondeterministic Finite Automata (NFA)

**Student:** Neilsen Vaz Â· **Roll No.:** 63 Â· **Class/Division:** T.E. Computer Engineering / D12A Â· **Semester:** V Â· **AY:** 2026â€“2027 Â· **Subject Code:** 26CMPC51

## Objective and model

Accept strings over `{a,b}` containing the substring `ab`. The NFA guesses where the substring begins.

## Files

- [63_Neilsen_Vaz_NFA_10-11-2026.jff](63_Neilsen_Vaz_NFA_10-11-2026.jff)

## JFLAP procedure

1. Open JFLAP 7.1.
2. Open the listed machine file(s) with **File â†’ Open**.
3. Use **Input â†’ Multiple Run** for automata and transducers; use the relevant grammar parse or TM run option for those machine types.
4. Compare outputs with the table below. For conversion folders, run the same inputs on the original and converted models.

## Test inputs and expected behavior

| Input | Expected behavior |
|---|---|
| `ab` | Accept |
| `aab` | Accept |
| `babb` | Accept |
| `Îµ` | Reject |
| `a` | Reject |
| `ba` | Reject |

## Verification status

Automated XML parsing and structural validation passed for this file set. Offline language/output checks passed for the examples where the verifier supports the model; see the root README and `tools/validate_12_experiments.py`. Exact DFA equivalence checks passed for the NFA-to-DFA and minimization pairs, and for the regex-to-DFA pair against the regex's direct language construction. DFA-to-grammar was checked by bounded derivation samples. Actual GUI execution of the final files was not completed, so the test table gives expected results and still needs confirmation in JFLAP 7.1.

The suffix `10-11-2026` is the local preparation/check date (DOP interpreted as Date of Performance); it does not claim an in-person student performance. Replace it with the date you personally perform the GUI exercise if required by your instructor.

## GUI Verification

NFA opened in JFLAP 7.1 and tested using **Input → Multiple Run**. All strings containing `ab` were accepted; strings without the substring were rejected as expected.

- `63_Neilsen_Vaz_NFA_10-11-2026.jff` — ✅ GUI-tested and verified.

### Screenshot

![NFA Multiple Run Result](63_Neilsen_Vaz_NFA_10-11-2026.png)