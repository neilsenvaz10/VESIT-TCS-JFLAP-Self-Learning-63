# Experiment 03: NFA to DFA Conversion

**Student:** Neilsen Vaz · **Roll No.:** 63 · **Class/Division:** T.E. Computer Engineering / D12A · **Semester:** V · **AY:** 2026–2027 · **Subject Code:** 26CMPC51

## Objective and model

Convert the NFA for binary strings ending in `01` by subset construction. The subset DFA accepts exactly the same language.

## Files

- [63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff](63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff)
- [63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff](63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff)

## JFLAP procedure

1. Open JFLAP 7.1.
2. Open the listed machine file(s) with **File → Open**.
3. Use **Input → Multiple Run** for automata and transducers; use the relevant grammar parse or TM run option for those machine types.
4. Compare outputs with the table below. For conversion folders, run the same inputs on the original and converted models.

## Test inputs and expected behavior

| Input | Expected behavior |
|---|---|
| `01` | Accept in both |
| `101` | Accept in both |
| `1101` | Accept in both |
| `ε` | Reject in both |
| `10` | Reject in both |
| `011` | Reject in both |

## Verification status

> **⚠️ Pending verification:** The converted DFA file was generated programmatically using subset construction logic. Automated XML parsing and structural validation passed, and offline equivalence checks confirmed both models accept the same strings for bounded-length inputs. However, the actual JFLAP GUI conversion process (Convert → Convert to DFA) has **not** been independently verified. The converted DFA file should be validated manually in JFLAP by running the original NFA through the subset construction tool and comparing the result.

Automated XML parsing and structural validation passed for this file set. Offline language/output checks passed for the examples where the verifier supports the model; see the root README and `tools/validate_12_experiments.py`. Exact DFA equivalence checks passed for the NFA-to-DFA and minimization pairs. Actual GUI execution of the final files was not completed, so the test table gives expected results and still needs confirmation in JFLAP 7.1.

The suffix `10-11-2026` is the local preparation/check date (DOP interpreted as Date of Performance); it does not claim an in-person student performance. Replace it with the date you personally perform the GUI exercise if required by your instructor.

## GUI verification (2026-11-11)

**Actual result:** Java 25 and `JFLAP7.1.jar` are installed, and a JFLAP 7.1 main window launched. The available GUI control session showed that window as disabled; menu clicks and keyboard input did not open an editor. Therefore none of the files below were opened in the editor, visually checked, run, or screenshotted in JFLAP during this session. No GUI test result is claimed.

- `63_Neilsen_Vaz_NFA_to_DFA_Converted_DFA_10-11-2026.jff` — **not opened in the JFLAP editor; not GUI-tested; no screenshot captured.**
- `63_Neilsen_Vaz_NFA_to_DFA_Original_NFA_10-11-2026.jff` — **not opened in the JFLAP editor; not GUI-tested; no screenshot captured.**

### Manual completion steps

1. Start JFLAP 7.1 and choose **File → Open**. Open the exact `.jff` file listed above.
2. Confirm the right editor opens (automaton, grammar, PDA, TM, transducer, or regex) and that its states/productions and labels are visible, readable, and not clipped.
3. Run every input in the test table using the editor's **Input** menu. Enter ε as an empty input. Record the result JFLAP actually displays; the table currently lists expected results only.
4. For this experiment's screenshot, capture the visible JFLAP editor after the model is open (and, if useful, a separate run result). Save genuine PNG captures in this folder as `gui_<JFF-base-name>.png`. Do not label a main-menu or file-manager image as a model screenshot.

Open both files separately. Run each test in the original NFA and the converted DFA; record whether both decisions match.

After performing the checks, replace each “not opened” status above with the observed result and add the genuine screenshot file link(s). Keep the expected-result table separate from actual observed results.
