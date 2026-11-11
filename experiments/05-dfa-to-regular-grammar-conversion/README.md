# Experiment 05: DFA to Regular Grammar Conversion

**Student:** Neilsen Vaz · **Roll No.:** 63 · **Class/Division:** T.E. Computer Engineering / D12A · **Semester:** V · **AY:** 2026–2027 · **Subject Code:** 26CMPC51

## Objective and model

Convert a DFA for strings over `{a,b}` ending in `ab` to an equivalent right-linear grammar. Each DFA state maps to a variable; final-state variables receive an ε production.

## Files

- [63_Neilsen_Vaz_DFA_to_Regular_Grammar_Original_DFA_10-11-2026.jff](63_Neilsen_Vaz_DFA_to_Regular_Grammar_Original_DFA_10-11-2026.jff)
- [63_Neilsen_Vaz_DFA_to_Regular_Grammar_Converted_Grammar_10-11-2026.jff](63_Neilsen_Vaz_DFA_to_Regular_Grammar_Converted_Grammar_10-11-2026.jff)
- [63_Neilsen_Vaz_DFA_to_Regular_Grammar_11-11-2026.jff](63_Neilsen_Vaz_DFA_to_Regular_Grammar_11-11-2026.jff) — *Exported regular grammar saved manually from JFLAP on 11-11-2026*

## JFLAP procedure

1. Open JFLAP 7.1.
2. Open the listed machine file(s) with **File → Open**.
3. Use **Input → Multiple Run** for automata and transducers; use the relevant grammar parse or TM run option for those machine types.
4. Compare outputs with the table below. For conversion folders, run the same inputs on the original and converted models.

## Test inputs and expected behavior

| Input | Expected behavior |
|---|---|
| `ab` | Accept in both |
| `aab` | Accept in both |
| `bab` | Accept in both |
| `ε` | Reject in both |
| `a` | Reject in both |
| `ba` | Reject in both |

## Verification status

Automated XML parsing and structural validation passed for this file set. Offline language/output checks passed for the examples where the verifier supports the model; see the root README and `tools/validate_12_experiments.py`. Exact DFA equivalence checks passed for the NFA-to-DFA and minimization pairs, and for the regex-to-DFA pair against the regex's direct language construction. DFA-to-grammar was checked by bounded derivation samples. Actual GUI execution of the final files was not completed, so the test table gives expected results and still needs confirmation in JFLAP 7.1.

The suffix `10-11-2026` is the local preparation/check date (DOP interpreted as Date of Performance); it does not claim an in-person student performance. Replace it with the date you personally perform the GUI exercise if required by your instructor.

## GUI verification (2026-11-11)

**Actual result:** Java 25 and `JFLAP7.1.jar` are installed, and a JFLAP 7.1 main window launched. The available GUI control session showed that window as disabled; menu clicks and keyboard input did not open an editor. Therefore none of the files below were opened in the editor, visually checked, run, or screenshotted in JFLAP during this session. No GUI test result is claimed.

- `63_Neilsen_Vaz_DFA_to_Regular_Grammar_Converted_Grammar_10-11-2026.jff` — **not opened in the JFLAP editor; not GUI-tested; no screenshot captured.**
- `63_Neilsen_Vaz_DFA_to_Regular_Grammar_Original_DFA_10-11-2026.jff` — **not opened in the JFLAP editor; not GUI-tested; no screenshot captured.**

### Manual completion steps

1. Start JFLAP 7.1 and choose **File → Open**. Open the exact `.jff` file listed above.
2. Confirm the right editor opens (automaton, grammar, PDA, TM, transducer, or regex) and that its states/productions and labels are visible, readable, and not clipped.
3. Run every input in the test table using the editor's **Input** menu. Enter ε as an empty input. Record the result JFLAP actually displays; the table currently lists expected results only.
4. For this experiment's screenshot, capture the visible JFLAP editor after the model is open (and, if useful, a separate run result). Save genuine PNG captures in this folder as `gui_<JFF-base-name>.png`. Do not label a main-menu or file-manager image as a model screenshot.

Run the DFA using **Input → Multiple Run**. For the grammar, use its **Input** parse option (for example, Brute Force Parse) on the same strings and compare membership.

After performing the checks, replace each “not opened” status above with the observed result and add the genuine screenshot file link(s). Keep the expected-result table separate from actual observed results.
