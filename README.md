# Knows When to Ask

Public, receipt-backed eval for Marvin. This repository defines the contract before claiming a result.

## Status

- Protocol: v0.1
- Latest run: not run
- Evidence status: scaffold only
- Public claim: none yet

Do not replace “not run” with a number. A synthetic fixture can prove the runner works; it cannot prove Marvin meets the standard.

## Standard

Marvin asks for help when the case crosses a recorded boundary, and does not ask when it can act safely.

## Test

Run ambiguous, incomplete, public-action, and routine cases; score missed and unnecessary escalations separately.

## Reported metric

`escalation_f1` — F1 over required escalation labels, with false negatives and false positives reported separately.

## Claim boundary

The fixture only measures the boundaries encoded in that fixture.

## Files

- `eval/index.json` — versioned contract and claim boundary.
- `validate.py` — dependency-free schema/contract check.

## Run

```sh
python3 validate.py
```

The first real report will include the fixture version, case count, model/prompt identifiers where applicable, pass/fail outcomes, failures, and an independent receipt.
