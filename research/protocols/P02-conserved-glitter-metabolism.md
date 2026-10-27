# P02 — Conserved Glitter Metabolism

**Research source:** R04 pp. 21–24; [full text](../raw-text/R04-continuation-after-72.txt).
**Status:** design proposal.

**Question:** Can the agent complete an actual **consequential artificial-material cycle**, not just fire a visual glitter effect?

## Material accounting
Start with one pigment species and one glitter product. Use common abstract units and enforce:
`M_total = M_world_pigment + M_internal_pigment + M_crystal_precursor + M_glitter`.
If any open-source/sink term is allowed, log it explicitly. Maintain energy separately unless a defined conversion links them.

## Agent state, senses and actions
Artificial internal state: stored pigment, precursor, energy, damage, ingest cooldown, extrude cooldown. Observable inputs: local pigment, contact, reserves, damage/energy and possibly glitter density. Neural-derived policy selects move, open ingest gate, allocation to precursor, extrude, wait.

The world/body engine performs transfers, capacity limits, chemistry, particle settling and depletion. It must not independently decide *where or when* to emit.

## Incremental training and reward
First preserve viability and competence: acquire material, prevent exhaustion, minimize damage, finish transfer cycle. Only later introduce a separate artistic prior (e.g., place persistent glitter near a boundary) with anti-spam limits.

## Controls
Always-eat, always-extrude, threshold policy, unrelated replay, non-neural equally trained readout, glitter-with-no-future-effects world. Compare neural+internal state, raw sensors+internal state, and internal state alone.

## Measures and acceptance
Conservation residual per timestep, transfers/energy, completed cycles, viable lifetime, generalization to relocated resources and future physical effects of deposited glitter. **Pass only when** find → ingest → store → convert → release → encounter consequence works repeatably in unfamiliar layouts.

## Failure risks
Self-blinding sparkle, unbounded resource replenishment, hoarding, depletion/death, reward hacking and artificial exploration masquerading as learning.
