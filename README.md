# Case-level Auditor Agreement Data

This repository contains supplementary case-level data for a
double-blind paper submission on automated auditing of medication
information in a healthcare Q&A corpus.

## Contents

- `table2_blind.csv` — 20 documents from a blind random review round
- `table3_purposive.csv` — 10 documents from a purposively sampled round

## Columns

| Column | Description |
|---|---|
| `case_id` | Document index within its round |
| `round` | `blind` or `purposive` |
| `rationale` | Condensed, translated reason for the expert's judgment |
| `type` | `S` = missing safety guidance, `X` = incomplete/ambiguous explanation, `C` = content error, `-` = no issue |
| `expert` | Clinical pharmacist's binary label (1 = requires revision) |
| `rule_based` | Rule-based auditor's label |
| `gpt5` | GPT-5 auditor's label |
| `claude` | Claude auditor's label |
| `gemini` | Gemini auditor's label |

## Note

Rationales are condensed and translated summaries of the expert
reviewer's reasoning, not verbatim source document text. This
repository is provided for review transparency and will be
finalized upon acceptance.
