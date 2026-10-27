# P01 — Bilateral Contour Grazer

**Research source:** R04 pp. 18–20; full text: [R04](../raw-text/R04-continuation-after-72.txt).
**Status:** design proposal, not implemented.
**Question:** Does the currently described bilateral escape-related neural circuit distinguish left/right synthetic boundary cues well enough to help an unfamiliar material task?

## Initial setup
- Small 2D arena, two pigment patches, persistent contour boundaries, one moving organism and a bounded action cost.
- Sample body-relative left/right boundary distance *or* pigment concentration at first, not several signals mixed together. Optionally add local curvature only after discrimination is established.
- Encode into existing verified neural input groups; name it **synthetic contour-to-looming-channel substitution**, not natural color/contour perception.
- Record left/right downstream populations and time windows separately; verify all named neurons against an actual circuit manifest.

## Stage A — sensory information test
Present mirrored stimuli across weak/medium/strong gains, no learning; test whether a tiny held-out classifier discriminates sides from *neural observations alone*. If not, repair the encoding before making a behavior model.

## Stage B — controller
Freeze the connectome graph. Fit small linear/logistic neural-feature decoder to a simple geometric teacher. Actions: turn left/right, advance, pause/graze. Then consider controlled readout RL separately.

## Controls
Matched rewired circuit + retrained decoder; raw left/right sensor values + decoder; time-shuffled neural features; mean-state neural features; simple scripted policy. Equal evaluation scenes/action budgets.

## Measures and acceptance
Held-out left/right accuracy; pigment per unit action cost; collisions; response latency; mirrored generalization; changed gains. **First criterion:** frozen readout improves over constant and timing-shuffled signals across held-out mirrored scenes. This would not prove biological perception or advantage over raw sensors.

## Known failure risks
Symmetric downstream responses; saturation; one neural population dominating; fixed turning loophole; decoder's own memory doing the work; local movement rules completing the task.
