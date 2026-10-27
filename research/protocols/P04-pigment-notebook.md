# P04 — Pigment Notebook (external memory)

**Research source:** R04 pp. 28–30; [full text](../raw-text/R04-continuation-after-72.txt).
**Status:** design proposal.

**Question:** Can the organism create an environmental trace that stores information and later use that information after its transient controller state has been reset?

## Arena and mechanism
An initial cue indicates which one of two later gates will be useful. Remove the cue before the decision. The organism may deposit and sense a pigment mark **or** change a channel/barrier so future flow encodes the earlier cue. Its neural-feature-based readout selects whether/where to mark and which gate to approach.

## Critical hidden-memory audit
Search for leakage through recurrent decoder state, smoothing, previous action, position history, RNG, episode labels, object IDs, provenance tags, train-state updates or a hidden `correctGate` value. Do not allow privileged bypasses.

## Factorial tests
- Transient state preserved, trace preserved.
- Transient state reset, trace preserved.
- Transient state preserved, trace erased.
- Transient state reset, trace erased.

Also swap marks between gates; use appearance-matched decoys; disable the marks' sensor effects while preserving rendered marks; and test invisible-but-sensable marks.

## Measures and acceptance
Gate choice after delay, cost, dependence on mark location/content, effect of mark swaps/erasures, recovery when internal transient state reset. **Pass only when** persistent marks carry usable information and disrupting or swapping them changes choices in the predicted direction.

**Interpretation limit:** external-memory use by the engineered hybrid, not “the fly invented writing.”
